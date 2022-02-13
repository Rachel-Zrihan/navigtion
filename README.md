# navigtion
add-safe-args:
add to project-level build.gardle:
	classpath "androidx.navigation:navigation-safe-args-gradle-plugin:2.4.0"
add to project-level build.gardle:
plugins:
apply plugin: 'kotlin-android'
apply plugin: 'kotlin-kapt'
apply plugin: 'kotlin-android-extensions'
apply plugin: "androidx.navigation.safeargs"



create navigation resource file
add destinations 
add arguments

for navigation:
val action = GameFragmentDirections.actionGameToScore()
action.score = viewModel.score.value!!
NavHostFragment.findNavController(this).navigate(action)
![image](https://user-images.githubusercontent.com/55790024/153771582-63cb08c8-004d-4787-8eaf-b16e63f7d072.png)
