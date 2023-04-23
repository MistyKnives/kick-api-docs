# Send Message
Send a message directly to a channel's chatroom
**URL**: `/api/v1/chat-messages`
**METHOD**: `POST`
**Rate Limited?**: `YES`
**Authenticated?**: `YES`

<details>
    <summary style="font-weight: bold">Paramaters</summary>

```json
{
    "chatroom_id": Long,
    "message": String,
}
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>

```json
{
    "chatroom_id": 124566,
    "message": "Hello Everyone!",
}
```
</details>

<details>
    <summary style="font-weight: bold">Response</summary>

```json
{
    "status": 200,
    "success": true,
    "message": "Message sent successfully"
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
</details>