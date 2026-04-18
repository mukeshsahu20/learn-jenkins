pipeline{

 agent any

 stages {'code quality'} {
  steps {
     echo 'code quality'
     }
  }

 stages {'style checks'} {
  steps {
  echo 'code quality'
   }
 }

  stages {'unit tests'} {
   steps {
   echo 'unit tests'
    }
  }

  stages {'Download dependencies'} {
  when { tag "*"}
   steps {
   echo 'Download dependencies only when there is Tag'
    }
  }

  stages {'Prepare artifact'} {
  when { tag "*"}
   steps {
   echo 'Prepare artifact only when tag is there '
    }
  }

    stages {'Publish artifact'} {
    when { tag "*"}
     steps {
     echo 'Publish artifact only when there is Tag'
      }
    }



}
