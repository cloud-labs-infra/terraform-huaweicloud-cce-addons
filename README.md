# Huawei Cloud Container Engine Add-ons

[Add-ons documentation](https://support.huaweicloud.com/intl/en-us/usermanual-cce/cce_10_0064.html)

To get information about add-on use the following data `huaweicloud_cce_addon_template`.

Example for `metrics-server` add-on

```hcl
data "huaweicloud_cce_addon_template" "test" {
  cluster_id = var.cce_cluster_id
  name       = "metrics-server"
  version    = "1.3.2"
}

output "version" {
  value = data.huaweicloud_cce_addon_template.test
}
```
