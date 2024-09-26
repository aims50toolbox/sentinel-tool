# AIMS AI Sentinel Tool

The tool provides object detection on images. The tool provides means to select certain classes to be detected.

## Usage
The tool can be used as a conventional AI tool (see the [AI Toolbox](https://github.com/aims50toolbox/aitoolbox)). You can experiment with the `query.ipynb` to check the tool capabilities. Also, you can deploy the tool as a REST service. Suppose, this tool is checked out into `~/aitools/sentinel`, then you can deploy it into `/tmp/sentinel_deploy` 
```
python3 -m aitoolbox deploy ~/aitools/sentinel -o /tmp/sentinel_deploy
```

After that, go to the deploy directory and build the image:
```
cd /tmp/sentinel_deploy
docker compose build
docker compose up
```

Running the service, you can test it with the provided `test/example.http` file and the Visual Code REST client extension.
