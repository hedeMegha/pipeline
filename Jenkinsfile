pipeline{
    agent any 

    parameters{
        string(name: "Username", defaultValue:"megha", description:"enter your name here")
        booleanParam(name:"Toggle", defaultValue: true, description: "true or false")
        text(name: "Details", defaultValue: "megha", description: "extra details here")
        choice(name: "Choice", choices:[ "one", "two", "three", "four"], description: "you have 4 choices")
        password(name: "Password", defaultValue: "secret", description: "enter your password here")
    }

    environment {
        TEST = "test_value"
    }
    stages{
        stage ('build'){
            steps{
                echo "$Username"
                echo "$Toggle"
                echo "$Details"
                echo "$Choice"
                echo "$Password"
            }
        }
    }
}