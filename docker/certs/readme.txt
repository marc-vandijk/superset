Frontend SSL Certificates


https://github.com/Subash/mkcert

Created these certificates with following commands (valid 10 years, so you probably wont have to do it):
--------------------------------------------------------
mkcert create-ca --organization "DWG" --country-code "NL" --state "Zuid-holland" --locality "Schiedam" --validity 3649
mkcert create-cert --validity 3649 --domains "localhost,127.0.0.1"


To install them:
--------------------------------------------------------
- For the frontend ssl, right click on the file DWG.TMS.Web\certs\ca.crt and choose "Install certificate"
- Choose "Local machine", next
- Place in certificate store "Trusted Root Certification Authorities" and finish
- Restart browser because it probably cached the previous certificate
