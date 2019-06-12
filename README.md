# TecholutionAssignment
Assignment to create a interface for uploading and downloading files using spring boot

Hi there...
I have only implemented the service layer for this application.
Two rest API's have been omplemented:
 1) Uploading file to AWS S3 bucket.
    Input -----> File in byte format, file name, folder and content type (Will be handled from the client -side)
    Output -------> ResponseDto: If the file has been successfully uploaded
                          Message = "file successfully uploaded to aws"
                          Status = "Success"
                          ReturnValue = 1
                    ResponseDto: If the file has not been successfully uploaded
                          Message = "Error uploading file"
                          Status = "Failure"
                          ReturnValue = 0
2) Generating AWS link of the required File.
    Input ------> Required file path and File Name
   Output -------> ResponseDto: If the file has been successfully uploaded
                          Message = "Successfully generated aws link"
                          Status = "Success"
                          ReturnValue = 1
                    ResponseDto: If the file has not been successfully uploaded
                          Message = "Error while generating aws link of file"
                          Status = "Failure"
                          ReturnValue = 0

