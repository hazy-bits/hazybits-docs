## auth
`auth` lambda function is used to generate temporary access keys for client application
that can be used to access AWS IoT infrastructure. Main goal is to establish web socket
communication channel to get async notifications from the cloud about processing
events.

## start
`start` lambda function is used to start an AWS Workflow. It acts as main entry
point to the cloud and actual processing starts with this lambda. It returns immediately,
returning unique ID of the started workflow.

## threshold
`threshold` lambda function performs threshold image processing operation over
specified image and passes black and white result to the next lambda in processing
pipeline.

## ocr
`ocr` lambda function performs OCR over specified image and stores recognized
textual data to the specified location.

!!! note
    It is expected that input image is processed for better OCR results.
