# Movies Review Database

ibmcloud ce application create --name movieapps \
    --image us.icr.io/${SN_ICR_NAMESPACE}/movieapps \
    --registry-secret icr-secret \
    --src https://github.com/gradezero/qkfls-Movie-Reviews-Database \
    --env CLOUDANT_URL=https://76838001-b883-444d-90d0-46f89e942a15-bluemix.cloudant.com \
    --env CLOUDANT_USERNAME=76838001-b883-444d-90d0-46f89e942a15-bluemix \
    --env CLOUDANT_PASSWORD=8fb6a16b48903e87b769e7f4968521e85c2394ed8f0e69b2769e56dcb27d2e76 \
    --env NLU_APIKEY=Ezo2LmXcHJ_bXmSHlAi1FxEcW8FiOY93a9bAkw-33Z-v \
    --env NLU_URL=https://api.au-syd.natural-language-understanding.watson.cloud.ibm.com/instances/cc926b38-f78f-4964-bd81-c254a9187eb5
