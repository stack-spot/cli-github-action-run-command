# cli-github-action-run-command

[![Action test](https://github.com/stack-spot/workflow-github-action-publish-content/actions/workflows/action-test.yml/badge.svg)](https://github.com/stack-spot/workflow-github-action-publish-content/actions/workflows/action-test.yml)

GitHub Action Run CLI Commands

## 📚 Usage

### Requirements

To learn more about generating account keys(`CLIENT_ID`, `CLIENT_KEY`, `REALM`), please refer to the documentation:
https://docs.stackspot.com/home/account/enterprise/service-credential

### Use Case

```yaml
    steps:
      - uses: stack-spot/cli-github-action-run-command@v1.0.0
        with:
          client_id: ${{ secrets.CLIENT_ID }}
          client_key: ${{ secrets.CLIENT_KEY }}
          realm: ${{ secrets.REALM }}
          workspace: workspace-y
          command_stk: "register app-deploy --version 1.0.0 --env dev --status succcess"
```


## License

[Apache License 2.0](https://github.com/stack-spot/publish-plugin-action/blob/main/LICENSE)


