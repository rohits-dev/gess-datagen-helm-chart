# gess-datagen-helm-chart
A Helm Chart to deploy https://hub.docker.com/r/rmoff/gess along with kafka pod to publish transaction data to Kafka.


# how to use the chart

helm repo add https://rohits.jfrog.io/artifactory/rs-helm rs-helm

helm upgrade -i gess-datagen



# package & publish
helm package .
curl -H "X-JFrog-Art-Api:<API_KEY>" -T <PATH_TO_FILE> "https://rohits.jfrog.io/artifactory/rs-helm/<TARGET_FILE_PATH>"