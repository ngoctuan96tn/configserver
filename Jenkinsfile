node {
    stage('clone git') {
        checkout scm
    }
    stage('start script') {
        steps {
            echo 'bat dau call api'
            def response = sh `curl --location --request GET 'https://reqres.in/api/users?page=2'`
            echo response

            echo 'done'
        }
    }
}