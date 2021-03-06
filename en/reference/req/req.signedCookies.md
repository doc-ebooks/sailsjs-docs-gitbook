# req.signedCookies
An object containing all the signed cookies from the request object. A signed cookie is protected against modification by the client. This protection is provided by a base64 encoded HMAC of the cookie value. When retrieving the cookie, if the HMAC signature does not match based on the cookie's value, then the cookie is not available as a member of the `req.signedCookies` object

### Purpose
An object containing all of the signed cookies from this request (`req`).


### Usage
```javascript
req.signedCookies;
```



### Example
Adding a signed cookie named "chocolatechip" with value "Yummy:

```javascript
res.cookie('chocolatechip', 'Yummy', {signed:true});
```

Retrieving the cookie:
```javascript
req.signedCookies.chocolatechip;
// "Yummy"
```







<docmeta name="uniqueID" value="reqsignedCookies113713">
<docmeta name="displayName" value="req.signedCookies">

