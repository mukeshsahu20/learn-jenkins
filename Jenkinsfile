pipeline{

 agent any

 stages

  stage{'code quality'} {
  steps {
     echo 'code quality'
     }
  }

 stage {'style checks'} {
  steps {
  echo 'code quality'
   }
 }

  stage {'unit tests'} {
   steps {
   echo 'unit tests'
    }
  }

  stage {'Download dependencies'} {
  when { tag "*"}
   steps {
   echo 'Download dependencies only when there is Tag'
    }
  }

  stage {'Prepare artifact'} {
  when { tag "*"}
   steps {
   echo 'Prepare artifact only when tag is there '
    }
  }

    stage {'Publish artifact'} {
    when { tag "*"}
     steps {
     echo 'Publish artifact only when there is Tag'
      }
    }



}
