Example:
>> docker build -t karthikdefaultregistry.azurecr.io/custom-ssh ./ 
>> docker run -p 4000:8080 karthikdefaultregistry.azurecr.io/custom-ssh (without exposing ssh port)
>> docker run -p 4000:8080 -p 2222:2222 karthikdefaultregistry.azurecr.io/custom-ssh (with ssh port being exposed)

Login to ssh on local machine:
>> ssh root@127.0.0.1 -p 2222 (default username and password on Azure will be "root" and "Docker!")