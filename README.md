<!-- BEGIN_TF_DOCS -->
# Terraform GitHub: Repositories

This is a GitHub module for deploying repositories.

[![Terraform Docs](https://github.com/fr-platform/terraform-github-repositories/actions/workflows/terraform-docs.yml/badge.svg)](https://github.com/fr-platform/terraform-github-repositories/actions/workflows/terraform-docs.yml)
[![Checkov](https://github.com/fr-platform/terraform-github-repositories/actions/workflows/checkov.yml/badge.svg)](https://github.com/fr-platform/terraform-github-repositories/actions/workflows/checkov.yml)

## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | ~> 1.2.0 |
| <a name="requirement_github"></a> [github](#requirement\_github) | ~> 4.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_github"></a> [github](#provider\_github) | 4.27.1 |

## Resources

| Name | Type |
|------|------|
| [github_branch_protection_v3.this](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/branch_protection_v3) | resource |
| [github_repository.this](https://registry.terraform.io/providers/integrations/github/latest/docs/resources/repository) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_repositories"></a> [repositories](#input\_repositories) | (Required) Map of map of repositories. | `map(map(any))` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_branches"></a> [branches](#output\_branches) | The list of this repositories' branches. |
| <a name="output_full_names"></a> [full\_names](#output\_full\_names) | Full names of the created repositories. |
| <a name="output_git_clone_urls"></a> [git\_clone\_urls](#output\_git\_clone\_urls) | URLs to clone the created repositories anonymously via the git protocol. |
| <a name="output_html_urls"></a> [html\_urls](#output\_html\_urls) | URLs to the created repositories on the web. |
| <a name="output_http_clone_urls"></a> [http\_clone\_urls](#output\_http\_clone\_urls) | URLs to clone the created repositories using HTTPS. |
| <a name="output_node_ids"></a> [node\_ids](#output\_node\_ids) | GraphQL global node ids for use with v4 API. |
| <a name="output_pages"></a> [pages](#output\_pages) | The block consisting of the repositories' GitHub Pages configuration. |
| <a name="output_repo_ids"></a> [repo\_ids](#output\_repo\_ids) | GitHub ID for the repositories. |
| <a name="output_ssh_clone_urls"></a> [ssh\_clone\_urls](#output\_ssh\_clone\_urls) | URLs to clone the created repositories using SSH. |
| <a name="output_svn_urls"></a> [svn\_urls](#output\_svn\_urls) | URLs to clone the created repositories via GitHub's Subversion protocol emulation. |
<!-- END_TF_DOCS -->