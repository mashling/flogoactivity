# Flogo Activity Gateway

## Install

To install run the following commands:
```
flogo create -f flogo.json
cd FlogoActivityGateway
flogo install github.com/pointlander/flogoactivity
flogo install github.com/TIBCOSoftware/flogo-contrib/activity/rest
flogo install github.com/TIBCOSoftware/flogo-contrib/activity/actreply
flogo install github.com/TIBCOSoftware/flogo-contrib/activity/log
flogo build
```

## Testing

Run:
```
FlogoActivityGateway
```

Then open another terminal and run:
```
curl http://localhost:9096/pets/1
```

You should then see something like:
```
{"category":{"id":0,"name":"string"},"id":1,"name":"aspen","photoUrls":["string"],"status":"done","tags":[{"id":0,"name":"string"}]}
```
