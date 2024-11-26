# Data model desgin

## Image

### Image model

| Field Name  | Data Type | Description                                                |
|-------------|-----------|------------------------------------------------------------|
| imageURL    | String    | Unique identifier for the image.                           |
| imageName   | String    | The name of the image file, used for display or debugging. |
| imagePath   | String    | AI-generated description of the image (processing result). |
| imageSize   | float     | Image size                                                 |
| imageWidth  | int       | Image width                                                |
| imageHeight | int       | Image height                                               |


### Image error model

| Field Name   | Data Type     | Description                                    |
|--------------|---------------|------------------------------------------------|
| imageURL     | String        | Unique identifier for the image.               |
| errorCode    | String        | Unique code representing the type of error.    |
| errorMessage | String        | Description of the error that occurred.        |
| errorTime    | LocalDateTime | Timestamp of when the error occurred.          |


## Item

### Item model


### Item error model

## AI