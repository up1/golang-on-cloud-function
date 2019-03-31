How to deploy on Google Cloud Function ?

```
$gcloud functions deploy hello --entry-point HelloWorld --runtime go111 --trigger-http
```

How to call function ?

```
curl https://us-central1-gitlab-203909.cloudfunctions.net/hello
```

How to load testing ?

```
$hey -n 5000 -c 10 https://us-central1-gitlab-203909.cloudfunctions.net/hello
```
