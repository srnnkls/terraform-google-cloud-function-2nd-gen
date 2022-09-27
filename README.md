# GCP Cloud Function 2nd gen

## Example

```HCL
module "otp-webhook" {
  source = "Polite-Code/cloud-function-2nd-gen/google"
  entry_point = "main"
  function_name = "otp-webhook"
  function_path = "../otp_webhook"
  project_id = var.project_id
  region = var.region
  runtime = "python310"
}
```