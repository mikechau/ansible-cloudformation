# Cloudformation Ansible Role

Ansible role for Cloudformation.

Currently only uploads a template to S3.

## Config Options

```yaml
##### Required

# The s3 bucket name.
cloudformation_s3_bucket: my-bucket-cloudformation

##### Options

# Set this if you want to use a specific AWS profile.
cloudformation_profile: my-aws-profile

# Set this if you want to specify a bucket region.
cloudformation_region: us-east-1

##### Defaults

# Base S3 path for the templates.
cloudformation_template_base_path: /templates

# List of templates to upload.
cloudformation_templates: []

# Enable server side encryption on the object.
cloudformation_template_encrypt: true

# Local path to the template directory.
cloudformation_template_dir: "{{ role_path }}/files/cf-templates"
```

