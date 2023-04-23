# User
Get the details of the username mentioned in the URL paramaters
**URL**: `/api/v1/users/{username}`
**METHOD**: `GET`
**Rate Limited?**: `YES`
**Authenticated?**: `NO`

<details>
    <summary style="font-weight: bold">Response</summary>
    
```json
{
    "id": Integer,
    "username": String,
    "bio": String,
    "twitter": String,
    "facebook": String,
    "instagram": String,
    "youtube": String,
    "discord": String,
    "tiktok": String,
    "profilepic": String
}
```
</details>

<details>
    <summary style="font-weight: bold">Example</summary>
    
```json 
{
    "id":842582,
    "username":"MistyKnives",
    "bio":"",
    "twitter":"MistyKnives",
    "facebook":"",
    "instagram":"MistyKnives",
    "youtube":"@MistyKnives",
    "discord":"",
    "tiktok":"MistyKnives",
    "profilepic":"https:\/\/kick-files-prod.s3.us-west-2.amazonaws.com\/images\/user\/842582\/profile_image\/conversion\/82d8365f-1ca8-487c-9cc4-914175f06f5a-fullsize.webp?X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENz%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJIMEYCIQCWSiipaUnOaDDH0T4fJ7x%2BxcPQvaw2OQwUoXvsRF%2BcqAIhAIpEb9Ulg30jnkPkgJFJP1qOehEGgT4eyNKmS8808unaKp4DCNX%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEQABoMMTk2MjMzNzc1NTE4IgzhFFPawoeX3%2B65W8Yq8gI0UQ%2BZNI2vErMLb1L2PdNcaB97d5zhuvStzSEbVGHbEyh1xaYYGkz2LEa52e%2BXpZI9M%2BW5sTGW3Rrzx5dVMbanNwEbYJHraSoGhBPPSqDWhYFtPvifG%2Frl9EjF1B4iPph1mUFSDjrbElfHavbVK1z4DRrRQ0n44P5hZFU3saW5Rsxv6KT4dpvlsHIMGKd7CR5dw0pw8uJS96cxzkZWSl9MnyW94%2FwPSvkvfncsIE3mWPH0%2FcwvSrTWdnQnQzlMfWEl%2F5Bs%2B7zXuLwo3vN%2FQomIMTL1EmJgWzBEzLulJvJ3VjCiR4XGJjhi9rFsj%2FUPzoRBuGjqxZv1XgUJICQZRSWQZZs8lKvVx91UX9l2%2FhMVDgyrNbFd2kuh3tjl96DyE%2BwL8vgDd9NaKS9q%2BlSErvVfLmam1f58YOcfJSEnjGitMTvLgokTfc%2BEZRoBRs3Z3l%2FdO6bqyMdqHW7NY6L16Hf2ntkyGpzWKHuOor5cXF2ubfVOMLvBlKIGOpwBuUHLyookr5rrXvFPetOa17Y5K3dlRYAMPukV0Uyn%2F3PHdHSe8aC20tp4dSotwRvvb9QNjfHIssemgPsJ0qH1Wg4OpFBPoFSyy9VfQnaNUPWtUKx49kNyOeJHg1Eswu3GvNEq46FU7aXX9JioL%2Bl%2FhBDOzbiHogr9S48Eq3jitj5gwzo2CrWbVEqwO%2B7AsSwd8XJybQW17fM0RVpv&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=ASIAS3MDRZGPGWIBDAF5%2F20230423%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20230423T122703Z&X-Amz-SignedHeaders=host&X-Amz-Expires=1200&X-Amz-Signature=d5d92b9721acb043efc69c473b3218f4ce3b383881e6e4382b9913fb9595d7bd"}
```
</details>

**Errors**:

| Error         | Response      | Reason |
| ------------- | ------------- | ------ |
| 404           | Not Found     | Account with 'username' was not found in the database. | 