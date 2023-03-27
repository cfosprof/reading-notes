# Class 15: Authentication

<details markdown="block"><summary>Things</summary>

### <li> Reading</li>



### <li> What is OAuth</li>

An open standard for authentication and authorization. It allows users to give third-party applications access to their data without having to give them their passwords.

### <li> Give an example of what using OAuth would look like.</li>

When a user logs into a website or application using their google account, they are using OAuth.

### <li> How does OAuth work? What are the steps that it takes to authenticate the user?</li>

By using accesss tokens. The user is redirected to the third-party application, where they are asked to log in. The third-party application then redirects the user back to the original application, along with an access token. The original application then uses the access token to access the user’s data.

### <li> What is OpenID?</li>

Is the standard for authentication. It allows users to log into third-party applications using their google account.

### <li> What is the difference between authorization and authentication?</li>

Authentication is the process of verifying who a user is. Authorization is the process of verifying what they have access to.

### <li> What is Authorization Code Flow?</li>

Is an oauth 2.0 flow that exchanges an authorization code for a token.

### <li> What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?</li>

Authorization Code Flow with PKCE is an oauth 2.0 flow that adds an extra layer of security to prevent code interception attacks. 

### <li> What is Implicit Flow with Form Post?</li>

An oauth 2.0 flow that allows clients to obtain an access token directly from the authorization server. It is used in single-page applications.

### <li> What is Client Credentials Flow?</li>

AN oauth 2.0 flow that allows clients to obtain an access token using only their client credentials.

### <li> What is Device Authorization Flow?</li>

An oauth 2.0 flow that allows clients to obtain an access token by asking the user to authorize on a different device.

### <li> What is Resource Owner Password Flow?</li>

An oauth 2.0 flow that allows clients to obtain an access token by asking the user for their credentials.

</details>
