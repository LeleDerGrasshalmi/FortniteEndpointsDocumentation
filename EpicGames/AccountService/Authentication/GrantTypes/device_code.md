## Account Service - Auth Grant: device_code

You may wanna checkout how to create one [here](../DeviceCode/Create.md). <br/>
You are meant to send this request in an interval (From the Device Code Response) until the Device Code has been accepted by the User.

### Body

`device_code`: The Code from before (from creation)
