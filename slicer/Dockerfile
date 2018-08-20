FROM rocker/tidyverse

RUN echo 'utils::setRepositories(ind=1:4)' > ~/.Rprofile

RUN /bin/bash -c 'git clone https://github.com/Stuartlab-UCSC/traj-converters.git'

RUN R -e 'install.packages(c("lle", "SLICER", "optparse","gam"))'
