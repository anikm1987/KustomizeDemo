# Example use case of kustomize

```
app1\base - contains base deployment config.

app1\overlays\dev - Contains instructions specific dev environment. It applies on top of base layer.

app1\overlays\staging - Contains instructions specific staging environment. It applies on top of dev layer, which in turn applies on base layer.

```

# Command to execute 

```
To run under base folder - 
C:\Aniket\technical\kustomize\Demo\app1\base> kustomize build

C:\Aniket\technical\kustomize\Demo\app1\overlays\dev> kustomize build

C:\Aniket\technical\kustomize\Demo\app1\overlays\staging> kustomize build

```