# nks-sample

## Chart? 作成中

先日のnginx-deploymentをそのままhelmの形に落とし込みたい  
枠については  
```
$ helm create nginx-sample
```
で作っただけ、そこに先日のdelpoyment.yamlとService.yamlに相当するものをrenameの上移動  
chartとしての体裁(deploy時に--setほにゃららでValueを変更できる形)には一切していない  
そもそもこの形にするだけで動くのか不明なので試す必要がある

### how to deploy LocalChart
$ helm install --name nginx-sample path/to/chart/nginx-sample

### dry run  
$ helm install --name nginx-sample path/to/chart/nginx-sample --dry-run --debug


