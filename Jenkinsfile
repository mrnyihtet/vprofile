pipeline { 
    agent any
    tools {
        maven "Maven3"
        jdk "OracleJDK8"
    }
    environment {
        SNAP_REPO = 'vprofile-snapshot'
        NEXUS_USER = 'admin'
        NEXUS_PASS = '@dmin1995'
        RELEASE_REPO = 'vprofile-release'
        CENTRAL_REPO = 'vprofile-proxy'
        NEXUSIP = '192.168.42.51'
        NEXUSPORT = '8081'
        NEXUS_GRP_REPO = 'vprofile-group'
    }
    stages { 
        stage ('Build') { 
            steps { 
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}
