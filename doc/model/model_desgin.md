# Data model desgin
## Image
### Image model

| Field Name    | Data Type     | Required | Description                                                                 |
|---------------|---------------|----------|-----------------------------------------------------------------------------|
| `imageURL`    | Long          | Yes      | Unique identifier for the image.                                            |
| `fileName`    | String        | Yes      | The name of the image file, used for display or debugging.                  |
| `filePath`    | String        | Yes      | The storage path of the image, pointing to its location in the file system. |
| `description` | String        | No       | AI-generated description of the image (processing result).                  |
| `uploadTime`  | LocalDateTime | Yes      | The time when the image was uploaded.                                       |

### Image error model

| Field Name     | Data Type     | Required | Description                                 |
|----------------|---------------|----------|---------------------------------------------|
| `imageURL`     | Long          | Yes      | ID of the associated image.                 |
| `errorCode`    | String        | Yes      | Unique code representing the type of error. |
| `errorMessage` | String        | Yes      | Description of the error that occurred.     |
| `errorTime`    | LocalDateTime | Yes      | Timestamp of when the error occurred.       |

## Item
### Item model

### Item error model

## AI