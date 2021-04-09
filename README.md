#### login to graphana | admin | admin

```
localhost:3000
```

#### click on 'Add your first data source'

#### select 'prometheus'

#### and add url in grafana

`http://prometheus:9090`

#### save & test

### import grafana dashboards

#### watch grafana dashboards

search: node exporter grafana dashboards

and watch 'Get this dashboard'

example (docker containers failed): 893


example1 (docker): 11600, 193
example2 (node-exporter): 1860



### Si tiene problemas con las metricas de CAdvisor y muestra 0 configure lo siguiente:

Agregar una configuracion al grupo de arranque

`nano /etc/default/grub`

editar la siguiente linea y agregar el siguiente contenido

```
GRUB_CMDLINE_LINUX_DEFAULT="cgroup_enable=memory swapaccount=1"
```

luego aplicar el grupo y reiniciar

`update-grub && reboot`