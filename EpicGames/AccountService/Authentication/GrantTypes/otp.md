## Account Service - Auth Grant: otp

Used for 2 FA Verification. (otp = One Time Password)

**Note**: You must use the same device id as the password request used to get the challenge.

### Body

`otp`: 2FA Verify Code <br/>
`challenge`: 2FA Challenge Id
