# API-Responses

package to keep all API standard codes and messages at one place.

How to use : 

Install package using : `npm i git+http://danish.galiyara:NHaBKpsXVkrkQKmUxest@git.vivaconnect.co/helo-whatsapp/api-responses.git`

After installing there are two options :

Option  1
```
const apiResponses = require('api-responses')

// inside the function to send out api response
__util.send(res, { type: apiResponses.SUCCESS, data: { token: token, emailVerifiedStatus: userData.email_verified === 1, phoneVerifiedStatus: userData.phone_verified === 1, tncAccepted: 
userData.tnc_accepted === 1, role: userData.role_name, tfaType: userData.tfa_type, tfaTypeDisplayName: userData.tfa_type_display_name } })
```

option 2 (handling in current approach)
```
inside constants.js
module.exports.RESPONSE_MESSAGES = require('api-responses')
# api-responses
