UBcp_geaRAGwbLdrbP9Jsw

curl -v https://login.salesforce.com/services/oauth2/token -d "grant_type=password" -d "client_id=<your_consumer_key>" -d "client_secret=<your_consumer_secret>" -d "username=<your_username>" -d "password=<your_password_and_security_token>" -H 'X-PrettyPrint:1'
