/*
 * See the documentation for more options:
 * https://github.com/jenkins-infra/pipeline-library/
 */
buildPlugin(
 useContainerAgent: true,
 configurations: [
  // Test the common case (i.e., a recent LTS release) on both Linux and Windows
  // with same core version as the lowest baseline requested by pom.xml
  [ platform: 'linux', jdk: '17', jenkins: '2.479.3' ],
  [ platform: 'windows', jdk: '17', jenkins: '2.479.3' ],

  // Test the bleeding edge of the compatibility spectrum (i.e., the latest supported Java runtime).
  // see also https://www.jenkins.io/doc/developer/plugin-development/choosing-jenkins-baseline/
  [ platform: 'linux', jdk: '21', jenkins: '2.484' ],
])
