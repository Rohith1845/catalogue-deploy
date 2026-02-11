@Library('Jenkins-shared-library') _

properties([
    parameters([
        string(name: 'appVersion' , value: "${appVersion}"),
        string(name: 'deploy_to' , value: "dev")
    ])
])

def configMap =[
        appVersion = configMap.get("appVersion"),
        project = configMap.get("project"),
        component = configMap.get("component"),
        deploy_to = configMap.get("deploy_to")
]

EKSDeploy(configMap)
