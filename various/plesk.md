# Plesk

Various stuff with Plesk.

## Error : 403 on static files on new installation

Happened while installing new websites through Plesk, with each CSS/Js files returning  ``` 403 Forbidden ```.

**Solution**

On Plesk, go to Domains -> Apache and Nginx settings, then untick ```Smart static files processing``` 