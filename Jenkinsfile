pipeline { 
    agent any
    tools {
        maven "Maven3"
        jdk "OracleJDK8"
    }
    environment {
        SNAP-REPO = 'vprofile-snapshot'
        NEXUS-USER = 'admin'
        NEXUS-PASS = '@dmin1995'
        RELEASE-REPO = 'vprofile-release'
        CENTRAL-REPO = 'vprofile-proxy'
        NEXUSIP = '192.168.42.51'
        NEXUSPORT = '8081'
        NEXUS-GRP-REPO = 'vprofile-group'
        NEXUS-LOGIN = 'nexus'
    }
    stages { 
        stage ('Build') { 
            steps { 
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}
