# esphome_configuration

Git repository containing my configuration for my ESPHome devices

Any variables that are shared across the devices are stored in secrets.yaml

Any device specific variables are stored in the substitutions at the top of the file to make
new device deployment simpler.

Use the following code to update all (assuming you are using fish):

```fish
for file in *.yaml
    esphome $file compile
    esphome $file upload
end
```
