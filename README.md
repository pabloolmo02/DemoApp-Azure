AZURE DEMO APP
1. CREAR GRUPO (location, name )


2. CREAR PLAN ( name, grupo recursos, location, “Precio”, S.O)
az appservice plan create --name funnyplan --resource-group funnygroup --location eastus --sku S1 --is-linux (para que lo cree en linux, si no se pone nada lo crea en Windows). 
Esto se crea desde el bash del portal de Azure, si fuese en VS no haría falta el $ para false

3. CREAR APP SERVICE ()
az webapp create --name demoappservice --plan demoplan --resource-group demogrupo0 --runtime dotnet:8
az webapp list-runtimes para ver los lenguajes según linux o windows

