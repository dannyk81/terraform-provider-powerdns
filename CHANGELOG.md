## 1.2.1 (Unreleased)
## 1.2.0 (October 11, 2019)

FEATURES:
  * **Added support for terraform resource import** ([#31](https://github.com/terraform-providers/terraform-provider-powerdns/issues/31))

FIXES:
  * **Validate value of records** - record with empty records deleted the record from the PowerDNS remote but not from state file ([#33](https://github.com/terraform-providers/terraform-provider-powerdns/issues/33))

## 1.1.0 (August 13, 2019)

FEATURES: 
  * **HTTPS Custom CA**: added option for custom Root CA for HTTPS Certificate validation (option `ca_certificate`) ([#22](https://github.com/terraform-providers/terraform-provider-powerdns/issues/22))
  * **HTTPS**: added option to skip HTTPS certificate validation - insecure HTTPS (option `insecure_https`) ([#22](https://github.com/terraform-providers/terraform-provider-powerdns/issues/22))

ENHANCEMENTS:
  * The provider doesn't attempt to connect to the PowerDNS endpoint if there is nothing to be done ([#24](https://github.com/terraform-providers/terraform-provider-powerdns/issues/24))
  * `server_url` (`PDNS_SERVER_URL`) can now be declared with/without scheme, port, trailing slashes or path ([#28](https://github.com/terraform-providers/terraform-provider-powerdns/issues/28))

## 1.0.0 (August 06, 2019)

NOTES:
 * provider: This release includes only a Terraform SDK upgrade with compatibility for Terraform v0.12. The provider remains backwards compatible with Terraform v0.11 and this update should have no significant changes in behavior for the provider. Please report any unexpected behavior in new GitHub issues (Terraform core: https://github.com/hashicorp/terraform/issues or Terraform PowerDNS Provider: https://github.com/terraform-providers/terraform-provider-powerdns/issues) ([#16](https://github.com/terraform-providers/terraform-provider-powerdns/issues/16))

ENHANCEMENTS:
  * Switch to go modules and Terraform v0.12 SDK [[#16](https://github.com/terraform-providers/terraform-provider-powerdns/issues/16)] 
  
## 0.2.0 (July 31, 2019)

FEATURES:
  * **New resource**: `powerdns_zone` ([#8](https://github.com/terraform-providers/terraform-provider-powerdns/issues/8))

ENHANCEMENTS:
  * resource/powerdns_record: Add support for set-ptr option ([#4](https://github.com/terraform-providers/terraform-provider-powerdns/issues/4))
  * build: Added docker-compose tests ([#9](https://github.com/terraform-providers/terraform-provider-powerdns/issues/9))

## 0.1.0 (June 21, 2017)

NOTES:

* Same functionality as that of Terraform 0.9.8. Repacked as part of [Provider Splitout](https://www.hashicorp.com/blog/upcoming-provider-changes-in-terraform-0-10/)
