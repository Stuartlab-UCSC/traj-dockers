#looks at requirments.txt and builds your python environment
FROM python:3.7
#
RUN git clone git://github.com/manusetty/wishbone.git

RUN pip install Cython && cd wishbone && pip3 install .

#opens a bash shell with -it
CMD ["/bin/bash"]

