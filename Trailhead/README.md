UBcp_geaRAGwbLdrbP9Jsw

CPDqx1QY5Q2V5EkxUMsddrDv

3MVG9szVa2RxsqBbPkWhxa9Op9C2LEqswMhxlaGAp3gyyyNGe5kdnGOCG5zfDoTq1JCu2pFiVgRsrstOa1BZS
3MVG9szVa2RxsqBbPkWhxa9Op9C2LEqswMhxlaGAp3gyyyNGe5kdnGOCG5zfDoTq1JCu2pFiVgRsrstOa1BZS

curl -v https://login.salesforce.com/services/oauth2/token -d "grant_type=password" -d "client_id=<your_consumer_key>" -d "client_secret=<your_consumer_secret>" -d "username=<your_username>" -d "password=<your_password_and_security_token>" -H 'X-PrettyPrint:1'

curl -v https://login.salesforce.com/services/oauth2/token -d "grant_type=password" -d "client_id=3MVG9szVa2RxsqBbPkWhxa9Op9C2LEqswMhxlaGAp3gyyyNGe5kdnGOCG5zfDoTq1JCu2pFiVgRsrstOa1BZS" -d "client_secret=998071830049976035" -d "username=vuk@crm.com" -d "password=Balkan2017CPDqx1QY5Q2V5EkxUMsddrDv" -H 'X-PrettyPrint:1'

```
Trying 136.147.42.44...
* TCP_NODELAY set
* Connected to login.salesforce.com (136.147.42.44) port 443 (#0)
* TLS 1.2 connection using TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384
* Server certificate: login.salesforce.com
* Server certificate: Symantec Class 3 Secure Server CA - G4
* Server certificate: VeriSign Class 3 Public Primary Certification Authority - G5
> POST /services/oauth2/token HTTP/1.1
> Host: login.salesforce.com
> User-Agent: curl/7.54.0
> Accept: */*
> X-PrettyPrint:1
> Content-Length: 213
> Content-Type: application/x-www-form-urlencoded
>
* upload completely sent off: 213 out of 213 bytes
< HTTP/1.1 200 OK
< Date: Fri, 08 Sep 2017 17:00:14 GMT
< Strict-Transport-Security: max-age=31536000; includeSubDomains
< X-Content-Type-Options: nosniff
< X-XSS-Protection: 1; mode=block
< Content-Security-Policy: referrer origin-when-cross-origin; upgrade-insecure-requests
< Set-Cookie: BrowserId=dqsPZkjIRVCnfA_DePlNTg;Path=/;Domain=.salesforce.com;Expires=Tue, 07-Nov-2017 17:00:14 GMT
< Expires: Thu, 01 Jan 1970 00:00:00 GMT
< Pragma: no-cache
< Cache-Control: no-cache, no-store
< X-ReadOnlyMode: false
< Cache-Control: no-store
< Content-Type: application/json;charset=UTF-8
< Vary: Accept-Encoding
< Transfer-Encoding: chunked
<
{
  "access_token" : "00D41000002m9QU!AQEAQKYewCxQ.EiCsCJGYhCxodw652x4FE4NaIOgbRIvmhORGTx0Ih2ohOLAWtLRS9pV474rxSPYWqcai6jOTrAc6LC90l8h",
  "instance_url" : "https://na35.salesforce.com",
  "id" : "https://login.salesforce.com/id/00D41000002m9QUEAY/005410000021HaPAAU",
  "token_type" : "Bearer",
  "issued_at" : "1504890014811",
  "signature" : "xloeMPDKqjr1NA1RdFWO1ggZE1WSjuqrF5vdppNzJh4="
* Connection #0 to host login.salesforce.com left intact
```
```curl
curl https://yourInstance.salesforce.com/services/apexrest/Cases/<Record_ID> -H 'Authorization: Bearer <your_session_id>' -H 'X-PrettyPrint:1'
```
