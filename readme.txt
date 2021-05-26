chief
currently trying a free style project gradle clean build, test, run
that works fine using 3 gradle tasks and a post guy.
so lets try it from a jenkins file.
fails
found: wipeout repository and force clone
i give up, writing the jenkins file in the jenkins job. 
doesn't seem to be any way to do that?
so try freestyel with git clone.
broke sample - tried to put in https://github.com/xvik/gradle-use-python-plugin/blob/master/README.md
fs1 still works  fine - it just make grdle calls.
running gralde from the command line in git bash fails.
A problem occurred evaluating project ':app'.
> Could not find method testImplementation() for arguments [org.junit.jupiter:junit-jupiter-api:5.7.1] on object of type org.gradle.api.internal.artifacts.dsl.dependencies.DefaultDependencyHandler.



