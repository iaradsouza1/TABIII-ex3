FROM frolvlad/alpine-miniconda3:python3.7

# install packages from bioconda
RUN conda install -c bioconda salmon fastqc
RUN pip install multiqc

# add bash for alpine / workaround because the base image is build from alpine
RUN /bin/sh -c "apk add --no-cache bash"