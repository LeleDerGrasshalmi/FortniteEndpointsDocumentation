## Account Service - Auth Grant: otp

Used for 2 FA Verification. (otp = One Time Password)

## Headers

`X-Epic-Device-ID`: A random value. This must be set to the same value used in the `password` request to get the challenge. If otp is successful, `password` requests made with the same device id will not be prompted for otp.

### Body

`otp`: 2FA Verify Code <br/>
`challenge`: 2FA Challenge Id
