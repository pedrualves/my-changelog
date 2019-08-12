# my-changelog

## a draft to generate changelogs

```git
url = git remote get-url origin

lastTag = git describe --abbrev=0 --tags

newTag = git tag -a v1.0 -m "msg"

git log HEAD --oneline --simplify-by-decoration --pretty=format:"* [%s](https://gitlab.produbanbr.corp/BR-SNT-ECT/GO-ECT-PCOR-AUTH-HANDLER/commits/%H)" > CHANGELOG.md 

git log HEAD --oneline --simplify-by-decoration --pretty=format:"* [%s](https://gitlab.produbanbr.corp/BR-SNT-MCP/java-mcp-api.git/commits/%H)" > CHANGELOG.md
```
