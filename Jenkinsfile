node {
    stage('SCM') {
        git credentialsId: '616a94de-85d0-4845-99e6-8cbb55d4c68e',
            url: 'git@github.com:padeoe/sakura-njunova-web.git'
    }

    stage("build") {
        sh 'gitbook build'
    }

    stage("deploy") {
        sshPublisher(
            publishers: [
                sshPublisherDesc(
                    configName: 'padeoe.com', 
                    transfers: [
                        sshTransfer(
                            excludes: '',
                            execCommand: '', 
                            execTimeout: 120000, 
                            flatten: false, 
                            makeEmptyDirs: false, 
                            noDefaultExcludes: false, 
                            patternSeparator: '[, ]+', 
                            remoteDirectory: '/var/www/html/sakura.njunova.com/public_html', 
                            remoteDirectorySDF: false, 
                            removePrefix: '_book', 
                            sourceFiles: '**/_book/**'
                        )
                    ], 
                    usePromotionTimestamp: false, 
                    useWorkspaceInPromotion: false, 
                    verbose: true
                )
            ]
        )
    }

}