on_commit {
  static_code_analysis()
}

on_pull_request to: develop, {
  static_code_analysis()
  build()
}

on_merge to: develop, {
  docker_local_deploy dev
}

// on_merge to: master, from: develop, {
//   docker_deploy_to prod
// }