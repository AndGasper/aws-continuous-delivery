# AWS CodePipeline
## Documentation
- [CodePipeline - Action Type](https://docs.aws.amazon.com/codepipeline/latest/userguide/integrations-action-type.html)

## Examples
- [CodePipeline - Tutorial: Create a Pipeline with an Amazon ECR Source and ECS-to-CodeDeploy Deployment](https://docs.aws.amazon.com/codepipeline/latest/userguide/tutorials-ecs-ecr-codedeploy.html)
- [CodePipeline - Create a Pipeline in CodePipeline That Uses Resources from Another AWS Account ](https://docs.aws.amazon.com/codepipeline/latest/userguide/pipelines-create-cross-account.html)


## Scratch Notes
- Stages:
    - 
        Name: StageName
        Actions: 
            - 
                Name: ActionName
                ActionTypeId:
                    Category: Deploy
                    Owner: AWS
                    Provider: CloudFormation
                    Version: '1'
                InputArtifacts
                    -
                        Name: ArtifactName
                Configuration:
                    ActionMode: CHANGE_SET_REPLACE | CREATE_STACK | UPDATE_STACK | DELETE_STACK | EXECUTE_CHANGE_SET | REPLACE_FAILED_STACK



REPLACE_FAILED_STACK

- CloudFormation Reports Failed States

```
enum FailedState {
    ROLLBACK_COMPLETE
    ROLLBACK_FAILED
    CREATE_FAILED
    DELETE_FAILED
    UPDATE_ROLLBACK_FAILED
}
```


```
Type: AWS::CodePipeline::Pipeline
Properties:
    ArtifactStore:
        ArtifactStore
    ArtifactStores:
        - ArtifactStoreMap
    DisableInboundStageTransitions:
        - StageTransition
    Name: String
    RestartExecutionOnUpdate
    RoleArn: String
    Stages:
        - StageDeclaration 
```

```
Stages:
    - StageDeclaration
```

```
Stages:
    -
        Actions:
            - ActionDeclaration
        Blockers:
            - BlockerDeclaration
        Name: String
```