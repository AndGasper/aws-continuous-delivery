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