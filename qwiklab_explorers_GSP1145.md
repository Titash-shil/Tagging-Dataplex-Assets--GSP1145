# Tagging Dataplex Assets || [GSP1145](https://www.cloudskillsboost.google/games/5178/labs/33840) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

### Run the following Commands in CloudShell
```
export LOCATION=
```
```
export ID=
```
```
gcloud dataplex lakes create orders-lake \
   --location=$LOCATION \
   --display-name="Orders Lake"


gcloud dataplex zones create customer-curated-zone \
    --location=$LOCATION \
    --lake=orders-lake \
    --display-name="Customer Curated Zone" \
    --type=CURATED \
    --resource-location-type=SINGLE_REGION


gcloud dataplex assets create customer-details-dataset \
--location=$LOCATION \
--lake=orders-lake \
--zone=customer-curated-zone \
--display-name="Customer Details Dataset" \
--resource-type=BIGQUERY_DATASET \
--resource-name=projects/$ID/datasets/customers


gcloud services enable datacatalog.googleapis.com
```
### #Follow the next step carefully from the video solution.

# Congratulations ..!! You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN)
