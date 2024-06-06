# Run this script to upload
aws lambda publish-layer-version --layer-name python-requests-layer \
    --zip-file fileb://layer_content.zip \
    --compatible-runtimes python3.11 \
    --compatible-architectures "arm64"

## Guide referenced here
https://docs.aws.amazon.com/lambda/latest/dg/python-layers.html