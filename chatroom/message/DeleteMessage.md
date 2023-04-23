# Send Message
Send a message directly to a channel's chatroom
<br>**URL**: `/api/v1/chat-messages/{messageId}`
<br>**METHOD**: `POST`
<br>**Rate Limited?**: `YES`
<br>**Authenticated?**: `YES`

<details>
    <summary style="font-weight: bold">Paramaters</summary>

```json
{
    "id": Long,
    "deleted": Boolean,
    "chatroom_id": Long
}
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>

```json
{
    "id": 122532,
    "deleted": true,
    "chatroom_id": 124566
}
```
</details>

<details>
    <summary style="font-weight: bold">Response</summary>

```json
{
    "status": 200,
    "success": true,
    "message": "Message deleted successfully"
}
```
</details>

<details>
    <summary style="font-weight: bold">Errors</summary>

```json
{
    "message":"The given data was invalid.",
    "errors": {
        "chatroom_id": [
            "The selected chatroom id is invalid."
        ]
    }
}

```

```json
{
    "message":"The given data was invalid.",
    "errors": {
        "id": [
            "The specified message id is invalid."
        ]
    }
}

```
</details>