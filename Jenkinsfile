node {
	stage ('Clone') {
        git url: 'https://github.com/Rupeshkryz/Pipeline_testing.git'
    }

    stage ("Upload file") {
        def uploadSpec = """{
            "files": [
                {
                    "pattern": "resources.txt",
                    "target": "Custom_testing"
                }
            ]
        }"""
        Server.upload spec: uploadSpec
    }
}