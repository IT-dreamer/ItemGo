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

| Field Name       | Data Type | Description               |
|------------------|-----------|---------------------------|
| shopId           | String    | fixed value               |
| ItemManageNumber | String    | Item manage number        |
| itemType         | Enum      | fixed value `Normal item` |
| itemTitle        | String    | Item title                |
| itemPrice        | String    | Item price                |
| pcDescription    | String    | Item description on PC    |
| spDescription    | String    | Same with pcDescription   |


### Item error model

| Field Name       | Data Type     | Description                                 |
|------------------|---------------|---------------------------------------------|
| ItemManageNumber | String        | Item manage number                          |
| errorCode        | String        | Unique code representing the type of error. |
| errorMessage     | String        | Description of the error that occurred.     |
| errorTime        | LocalDateTime | Timestamp of when the error occurred.       |

## AI

### AI model

| Field Name  | Data Type          | Description                                |
|-------------|--------------------|--------------------------------------------|
| imageURL    | List&lt;String&gt; | The URLs of the images                     |
| options     | List&lt;String&gt; | Keywords to be included in the description |
| description | String             | The description of the items               |

### error model
| Field Name   | Data Type     | Description                                    |
|--------------|---------------|------------------------------------------------|
| errorCode    | String        | Unique code representing the type of error.    |
| errorMessage | String        | Description of the error that occurred.        |
| errorTime    | LocalDateTime | Timestamp of when the error occurred.          |