pipeline { 
    agent any
    tools {
        maven "Maven3"
        jdk "OracleJDK8"
    }
    environment {
        SNAP_REPO = 'vprofile-snapshot'
<<<<<<< HEAD
        NEXUS_USER = admin
=======
        NEXUS_USER = 'admin'
>>>>>>> f2d57a38c8ebb11ae24782a79a5cff995cf62134
        NEXUS_PASS = '@dmin1995'
        RELEASE_REPO = 'vprofile-release'
        CENTRAL_REPO = 'vprofile-proxy'
        NEXUS_IP = '192.168.42.51'
        NEXUS_PORT = '8081'
        NEXUS_GRP_REPO = 'vprofile-group'
        NEXUS_LOGIN = 'nexus'
    }
    stages { 
        stage ('Build') { 
            steps { 
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}
