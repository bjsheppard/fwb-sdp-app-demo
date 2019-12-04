// static_code_analysis()
// build()

on_commit {
    static_code_analysis()
}

on_pull_request to: develop, {
  continuous_integration()
}

// on_merge_to: develop {
//   docker_deploy_to dev
// }

// on_merge to: master, from: develop, {
//   docker_deploy_to prod
// }