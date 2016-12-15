# Welcome to Service Bits Cloud

## Source code
We use BitBucket to host all repositories for the project. So far we have the
following repose (names **should** be changed!):

 * `aws-lambda-dev` - small repsitory with Dockerfile that allows to build AWS
 Linux environment to compile our native dependencies.
 * `aws-tesseract` - node js module for Tesseract OCR engine
 * `cloud-ocr` - set of lambda functions that perform image processing.
 * `documentation` - public web site with documentation related to the project.
 * `service-bits-web` - public web site that advertises Service Bits Cloud and
 allows to try our services online (perform OCR, image processing, etc.)

## Builds
We heavily rely on BitBucket Pipelines infracturure to build our aftifacts. So
far we have two configured builds (there should be more!):

 * `aws-tesseract` repo defines a pipeline for building node js Tesseract OCR engine
 using Docket image from `aws-lambda-dev` repo.
 * `documentation` repo defines a pipeline to build ourdocumentation pages using
 mkDocs.
