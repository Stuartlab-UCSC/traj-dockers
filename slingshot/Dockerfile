FROM rocker/tidyverse

RUN echo 'utils::setRepositories(ind=1:4)' > ~/.Rprofile

# Some dependencies of slingshot that need to be installed first.
RUN R -e 'install.packages(c("NMF","flexmix","dendextend"))'

RUN apt-get install -y libxml2-dev \
	libfreetype6-dev \
	libglu1-mesa-dev \ 
    r-cran-rgl

RUN R -e 'install.packages(c("optparse","gam"));source("https://bioconductor.org/biocLite.R");biocLite("kstreet13/slingshot")'
