



<!DOCTYPE html>
<html class="gl-light ui-green with-top-bar " lang="en">
<head prefix="og: http://ogp.me/ns#">
<meta charset="utf-8">
<meta content="IE=edge" http-equiv="X-UA-Compatible">
<meta content="width=device-width, initial-scale=1" name="viewport">
<title>docker/README.md · pavlin_yolov10_v11 · AI / Lab / AI Drone / Nvidia Jetson · GitLab</title>
<script>
//<![CDATA[
window.gon={};gon.api_version="v4";gon.default_avatar_url="https://gitlab.od.atncorp.com/assets/no_avatar-849f9c04a3a0d0cea2424ae97b27447dc64a7dbfae83c036c45b403392f0e8ba.png";gon.max_file_size=500;gon.asset_host=null;gon.webpack_public_path="/assets/webpack/";gon.relative_url_root="";gon.user_color_mode="gl-light";gon.user_color_scheme="solarized-dark";gon.markdown_surround_selection=true;gon.markdown_automatic_lists=true;gon.math_rendering_limits_enabled=true;gon.recaptcha_api_server_url="https://www.recaptcha.net/recaptcha/api.js";gon.recaptcha_sitekey=null;gon.gitlab_url="https://gitlab.od.atncorp.com";gon.promo_url="https://about.gitlab.com";gon.forum_url="https://forum.gitlab.com";gon.docs_url="https://docs.gitlab.com";gon.revision="2c7e66ebdb6";gon.feature_category="source_code_management";gon.gitlab_logo="/assets/gitlab_logo-2957169c8ef64c58616a1ac3f4fc626e8a35ce4eb3ed31bb0d873712f2a041a0.png";gon.secure=true;gon.sprite_icons="/assets/icons-50888ef7fb46c3a1fb53bc67cfc1085be59395f0d49dd55cdd8a8e269dede05b.svg";gon.sprite_file_icons="/assets/file_icons/file_icons-7cd3d6c3b29a6d972895f36472978a4b5adb4b37f9b5d0716a380e82389f7e0e.svg";gon.emoji_sprites_css_path="/assets/emoji_sprites-d746ae2450a3e9c626d338d77a101b84ff33a47c0c281b676d75c4a6ed2948a4.css";gon.gridstack_css_path="/assets/lazy_bundles/gridstack-5fcfd4ffbea1db04eaf7f16521bcab19ae3af042c8b4afe8d16781eda5a70799.css";gon.test_env=false;gon.disable_animations=false;gon.suggested_label_colors={"#cc338b":"Magenta-pink","#dc143c":"Crimson","#c21e56":"Rose red","#cd5b45":"Dark coral","#ed9121":"Carrot orange","#eee600":"Titanium yellow","#009966":"Green-cyan","#8fbc8f":"Dark sea green","#6699cc":"Blue-gray","#e6e6fa":"Lavender","#9400d3":"Dark violet","#330066":"Deep violet","#36454f":"Charcoal grey","#808080":"Gray"};gon.first_day_of_week=1;gon.time_display_relative=true;gon.time_display_format=0;gon.ee=false;gon.jh=false;gon.dot_com=false;gon.uf_error_prefix="UF";gon.pat_prefix="glpat-";gon.keyboard_shortcuts_enabled=true;gon.diagramsnet_url="https://embed.diagrams.net";gon.version="17.4.2";gon.current_user_id=109;gon.current_username="ppenev";gon.current_user_fullname="Pavlin Penev";gon.current_user_avatar_url=null;gon.features={"sourceEditorToolbar":false,"vscodeWebIde":true,"uiForOrganizations":false,"organizationSwitching":false,"removeMonitorMetrics":true,"explainCodeChat":false};
//]]>
</script>
<script>
//<![CDATA[
window.uploads_path = "/ai/lab/ai_drone/nvidia-jetson/uploads";



//]]>
</script>

<script>
//<![CDATA[
var gl = window.gl || {};
gl.startup_calls = {"/ai/lab/ai_drone/nvidia-jetson/-/blob/pavlin_yolov10_v11/docker/README.md?format=json\u0026viewer=rich":{}};
gl.startup_graphql_calls = [{"query":"query getBlobInfo(\n  $projectPath: ID!\n  $filePath: [String!]!\n  $ref: String!\n  $refType: RefType\n  $shouldFetchRawText: Boolean!\n) {\n  project(fullPath: $projectPath) {\n    __typename\n    id\n    repository {\n      __typename\n      empty\n      blobs(paths: $filePath, ref: $ref, refType: $refType) {\n        __typename\n        nodes {\n          __typename\n          id\n          webPath\n          name\n          size\n          rawSize\n          rawTextBlob @include(if: $shouldFetchRawText)\n          fileType\n          language\n          path\n          blamePath\n          editBlobPath\n          gitpodBlobUrl\n          ideEditPath\n          forkAndEditPath\n          ideForkAndEditPath\n          codeNavigationPath\n          projectBlobPathRoot\n          forkAndViewPath\n          environmentFormattedExternalUrl\n          environmentExternalUrlForRouteMap\n          canModifyBlob\n          canModifyBlobWithWebIde\n          canCurrentUserPushToBranch\n          archived\n          storedExternally\n          externalStorage\n          externalStorageUrl\n          rawPath\n          replacePath\n          pipelineEditorPath\n          simpleViewer {\n            fileType\n            tooLarge\n            type\n            renderError\n          }\n          richViewer {\n            fileType\n            tooLarge\n            type\n            renderError\n          }\n        }\n      }\n    }\n  }\n}\n","variables":{"projectPath":"ai/lab/ai_drone/nvidia-jetson","ref":"pavlin_yolov10_v11","refType":null,"filePath":"docker/README.md","shouldFetchRawText":false}}];

if (gl.startup_calls && window.fetch) {
  Object.keys(gl.startup_calls).forEach(apiCall => {
   gl.startup_calls[apiCall] = {
      fetchCall: fetch(apiCall, {
        // Emulate XHR for Rails AJAX request checks
        headers: {
          'X-Requested-With': 'XMLHttpRequest'
        },
        // fetch won’t send cookies in older browsers, unless you set the credentials init option.
        // We set to `same-origin` which is default value in modern browsers.
        // See https://github.com/whatwg/fetch/pull/585 for more information.
        credentials: 'same-origin'
      })
    };
  });
}
if (gl.startup_graphql_calls && window.fetch) {
  const headers = {"X-CSRF-Token":"YVubG9PtbucQqo44xeQDyBymFYvIZc9veWeEAIyrsbCJrnzmYgIZd7Em3GF-Xcr8jrFYArPnJAJx7J20lkXJ1w","x-gitlab-feature-category":"source_code_management"};
  const url = `https://gitlab.od.atncorp.com/api/graphql`

  const opts = {
    method: "POST",
    headers: {
      "Content-Type": "application/json",
      ...headers,
    }
  };

  gl.startup_graphql_calls = gl.startup_graphql_calls.map(call => ({
    ...call,
    fetchCall: fetch(url, {
      ...opts,
      credentials: 'same-origin',
      body: JSON.stringify(call)
    })
  }))
}


//]]>
</script>

<link rel="prefetch" href="/assets/webpack/monaco.b232988e.chunk.js">

<link rel="stylesheet" href="/assets/application-857280eb2c5ebf3a21350a6acc823e0b28bf87da97bda46f8d475bab7806dc71.css" />
<link rel="stylesheet" href="/assets/page_bundles/tree-613f28b9f7d3865f97b3a25cecb0fc0c1a43a14848d62b1ddf7a45839cd46496.css" /><link rel="stylesheet" href="/assets/page_bundles/projects-61bae953244f300140901fa29f63fbd0ecf2ddc06f150ed34dad3e59368e9a02.css" /><link rel="stylesheet" href="/assets/page_bundles/commit_description-065c52911d70ac846b47cc0f64e7a6e0d3daadd0cd34f5788259712569dc0dc3.css" /><link rel="stylesheet" href="/assets/page_bundles/work_items-1df2eea09269b0096c89bcdeba7f775c344c607599d35c3e540bd969463a3bd4.css" /><link rel="stylesheet" href="/assets/page_bundles/notes_shared-bb04929b630340c7b337fb6bfa30ea2d10fcfe6334e1c2e804a3159fc888c146.css" />
<link rel="stylesheet" href="/assets/application_utilities-0f64530bdd1cd7f39aa00294ccb76cb9a4a8a8d4fbe2f0f3479997820877adc1.css" />
<link rel="stylesheet" href="/assets/tailwind-df73256c46d660e287677379ab8d61af8585b74ed0a6d7a788608afecccfd1fb.css" />


<link rel="stylesheet" href="/assets/fonts-fae5d3f79948bd85f18b6513a025f863b19636e85b09a1492907eb4b1bb0557b.css" />
<link rel="stylesheet" href="/assets/highlight/themes/solarized-dark-00d8ec65284550069a669f9feae848bb528021c3af5cccc53e66e858d4c52e64.css" />


<link rel="preload" href="/assets/application_utilities-0f64530bdd1cd7f39aa00294ccb76cb9a4a8a8d4fbe2f0f3479997820877adc1.css" as="style" type="text/css">
<link rel="preload" href="/assets/application-857280eb2c5ebf3a21350a6acc823e0b28bf87da97bda46f8d475bab7806dc71.css" as="style" type="text/css">
<link rel="preload" href="/assets/highlight/themes/solarized-dark-00d8ec65284550069a669f9feae848bb528021c3af5cccc53e66e858d4c52e64.css" as="style" type="text/css">




<script src="/assets/webpack/runtime.bb284101.bundle.js" defer="defer"></script>
<script src="/assets/webpack/main.018e6284.chunk.js" defer="defer"></script>
<script src="/assets/webpack/graphql.e1f11a07.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.admin.abuse_reports.show-pages.dashboard.issues-pages.dashboard.milestones.show-pages.-13e11bbf.94a09ab2.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.admin.abuse_reports.show-pages.dashboard.issues-pages.groups.boards-pages.groups.infra-bae5b164.e1eb380e.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.admin.abuse_reports.show-pages.dashboard.issues-pages.groups.boards-pages.groups.issue-8dfa5f96.74f9ae83.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.admin.abuse_reports.show-pages.dashboard.issues-pages.groups.boards-pages.groups.issue-f804d6c2.35419d5c.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.groups.harbor.repositories-pages.groups.new-pages.groups.packages-pages.groups.registr-c21f1c50.0fbb41f2.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.search.show-super_sidebar.599796f4.chunk.js" defer="defer"></script>
<script src="/assets/webpack/super_sidebar.a1cd5f8e.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects-pages.projects.activity-pages.projects.alert_management.details-pages.project-ee413973.db11e848.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.admin.runners.show-pages.clusters.agents.dashboard-pages.dashboard.groups.index-pages.-d17ea602.9eaa870f.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects.blob.show-pages.projects.branches.new-pages.projects.commits.show-pages.proje-81161c0b.7e968083.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects.blob.show-pages.projects.show-pages.projects.snippets.edit-pages.projects.sni-42df7d4c.2c0bbb38.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects.blob.show-pages.projects.show-pages.projects.snippets.show-pages.projects.tre-c684fcf6.8bf42713.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects.blob.show-pages.projects.forks.new-pages.projects.show-pages.projects.tree.show.2300d4b7.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects.blob.show-pages.projects.show-pages.projects.tree.show.bec15eb6.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects.blob.show-pages.projects.tree.show-treeList.9861aec6.chunk.js" defer="defer"></script>
<script src="/assets/webpack/commons-pages.projects.blob.show-pages.projects.commits.show-pages.projects.compare.show.cdfd407a.chunk.js" defer="defer"></script>
<script src="/assets/webpack/pages.projects.blob.show.4479a877.chunk.js" defer="defer"></script>

<meta content="object" property="og:type">
<meta content="GitLab" property="og:site_name">
<meta content="docker/README.md · pavlin_yolov10_v11 · AI / Lab / AI Drone / Nvidia Jetson · GitLab" property="og:title">
<meta content="GitLab Community Edition" property="og:description">
<meta content="https://gitlab.od.atncorp.com/assets/twitter_card-570ddb06edf56a2312253c5872489847a0f385112ddbcd71ccfa1570febab5d2.jpg" property="og:image">
<meta content="64" property="og:image:width">
<meta content="64" property="og:image:height">
<meta content="https://gitlab.od.atncorp.com/ai/lab/ai_drone/nvidia-jetson/-/blob/pavlin_yolov10_v11/docker/README.md" property="og:url">
<meta content="summary" property="twitter:card">
<meta content="docker/README.md · pavlin_yolov10_v11 · AI / Lab / AI Drone / Nvidia Jetson · GitLab" property="twitter:title">
<meta content="GitLab Community Edition" property="twitter:description">
<meta content="https://gitlab.od.atncorp.com/assets/twitter_card-570ddb06edf56a2312253c5872489847a0f385112ddbcd71ccfa1570febab5d2.jpg" property="twitter:image">

<meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="138apbyJO3IrZp_ZHHWN_LpUkiXK0YrTCErjyOOfiLM_iv1YDWZM4orqzYCnzETIKEPfrLFTYb4Awfp8-XHw1A" />
<meta name="csp-nonce" />
<meta name="action-cable-url" content="/-/cable" />
<link href="/-/manifest.json" rel="manifest">
<link rel="icon" type="image/png" href="/assets/favicon-72a2cad5025aa931d6ea56c3201d1f18e68a8cd39788c7c80d5b2b82aa5143ef.png" id="favicon" data-original-href="/assets/favicon-72a2cad5025aa931d6ea56c3201d1f18e68a8cd39788c7c80d5b2b82aa5143ef.png" />
<link rel="apple-touch-icon" type="image/x-icon" href="/assets/apple-touch-icon-b049d4bc0dd9626f31db825d61880737befc7835982586d015bded10b4435460.png" />
<link href="/search/opensearch.xml" rel="search" title="Search GitLab" type="application/opensearchdescription+xml">




<meta content="GitLab Community Edition" name="description">
<meta content="#0e4328" name="theme-color">
</head>

<body class="tab-width-8 gl-browser-chrome gl-platform-windows" data-find-file="/ai/lab/ai_drone/nvidia-jetson/-/find_file/pavlin_yolov10_v11" data-group="ai_drone" data-group-full-path="ai/lab/ai_drone" data-namespace-id="618" data-page="projects:blob:show" data-page-type-id="pavlin_yolov10_v11/docker/README.md" data-project="nvidia-jetson" data-project-full-path="ai/lab/ai_drone/nvidia-jetson" data-project-id="524">

<script>
//<![CDATA[
gl = window.gl || {};
gl.client = {"isChrome":true,"isWindows":true};


//]]>
</script>


<div class="layout-page page-with-super-sidebar">
<aside class="js-super-sidebar super-sidebar super-sidebar-loading" data-command-palette="{&quot;project_files_url&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/files/pavlin_yolov10_v11?format=json&quot;,&quot;project_blob_url&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/blob/pavlin_yolov10_v11&quot;}" data-force-desktop-expanded-sidebar="" data-is-saas="false" data-root-path="/" data-sidebar="{&quot;whats_new_most_recent_release_items_count&quot;:7,&quot;whats_new_version_digest&quot;:&quot;618ce5f0030591b417694ba96ae6915ced5fcb4510912f752857458c059771c8&quot;,&quot;is_logged_in&quot;:true,&quot;context_switcher_links&quot;:[{&quot;title&quot;:&quot;Your work&quot;,&quot;link&quot;:&quot;/&quot;,&quot;icon&quot;:&quot;work&quot;},{&quot;title&quot;:&quot;Explore&quot;,&quot;link&quot;:&quot;/explore&quot;,&quot;icon&quot;:&quot;compass&quot;},{&quot;title&quot;:&quot;Profile&quot;,&quot;link&quot;:&quot;/-/user_settings/profile&quot;,&quot;icon&quot;:&quot;profile&quot;},{&quot;title&quot;:&quot;Preferences&quot;,&quot;link&quot;:&quot;/-/profile/preferences&quot;,&quot;icon&quot;:&quot;preferences&quot;}],&quot;current_menu_items&quot;:[{&quot;id&quot;:&quot;project_overview&quot;,&quot;title&quot;:&quot;Nvidia Jetson&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:524,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-project&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;manage_menu&quot;,&quot;title&quot;:&quot;Manage&quot;,&quot;icon&quot;:&quot;users&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/activity&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;activity&quot;,&quot;title&quot;:&quot;Activity&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/activity&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-project-activity&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;members&quot;,&quot;title&quot;:&quot;Members&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/project_members&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;labels&quot;,&quot;title&quot;:&quot;Labels&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/labels&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;plan_menu&quot;,&quot;title&quot;:&quot;Plan&quot;,&quot;icon&quot;:&quot;planning&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/issues&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;project_issue_list&quot;,&quot;title&quot;:&quot;Issues&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/issues&quot;,&quot;pill_count&quot;:&quot;0&quot;,&quot;link_classes&quot;:&quot;shortcuts-issues has-sub-items&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;boards&quot;,&quot;title&quot;:&quot;Issue boards&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/boards&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-issue-boards&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;milestones&quot;,&quot;title&quot;:&quot;Milestones&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/milestones&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;project_wiki&quot;,&quot;title&quot;:&quot;Wiki&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/wikis/home&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-wiki&quot;,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;code_menu&quot;,&quot;title&quot;:&quot;Code&quot;,&quot;icon&quot;:&quot;code&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/merge_requests&quot;,&quot;is_active&quot;:true,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;project_merge_request_list&quot;,&quot;title&quot;:&quot;Merge requests&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/merge_requests&quot;,&quot;pill_count&quot;:&quot;0&quot;,&quot;link_classes&quot;:&quot;shortcuts-merge_requests&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;files&quot;,&quot;title&quot;:&quot;Repository&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/tree/pavlin_yolov10_v11&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-tree&quot;,&quot;is_active&quot;:true},{&quot;id&quot;:&quot;branches&quot;,&quot;title&quot;:&quot;Branches&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/branches&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;commits&quot;,&quot;title&quot;:&quot;Commits&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/commits/pavlin_yolov10_v11&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-commits&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;tags&quot;,&quot;title&quot;:&quot;Tags&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/tags&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;graphs&quot;,&quot;title&quot;:&quot;Repository graph&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/network/pavlin_yolov10_v11&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-network&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;compare&quot;,&quot;title&quot;:&quot;Compare revisions&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/compare?from=main\u0026to=pavlin_yolov10_v11&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;project_snippets&quot;,&quot;title&quot;:&quot;Snippets&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/snippets&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-snippets&quot;,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;build_menu&quot;,&quot;title&quot;:&quot;Build&quot;,&quot;icon&quot;:&quot;rocket&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/pipelines&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;pipelines&quot;,&quot;title&quot;:&quot;Pipelines&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/pipelines&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-pipelines&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;jobs&quot;,&quot;title&quot;:&quot;Jobs&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/jobs&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-builds&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;pipelines_editor&quot;,&quot;title&quot;:&quot;Pipeline editor&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/ci/editor?branch_name=pavlin_yolov10_v11&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;pipeline_schedules&quot;,&quot;title&quot;:&quot;Pipeline schedules&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/pipeline_schedules&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-builds&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;artifacts&quot;,&quot;title&quot;:&quot;Artifacts&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/artifacts&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-builds&quot;,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;secure_menu&quot;,&quot;title&quot;:&quot;Secure&quot;,&quot;icon&quot;:&quot;shield&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/security/configuration&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;configuration&quot;,&quot;title&quot;:&quot;Security configuration&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/security/configuration&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;deploy_menu&quot;,&quot;title&quot;:&quot;Deploy&quot;,&quot;icon&quot;:&quot;deployments&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/releases&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;releases&quot;,&quot;title&quot;:&quot;Releases&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/releases&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-deployments-releases&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;feature_flags&quot;,&quot;title&quot;:&quot;Feature flags&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/feature_flags&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-feature-flags&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;packages_registry&quot;,&quot;title&quot;:&quot;Package Registry&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/packages&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-container-registry&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;container_registry&quot;,&quot;title&quot;:&quot;Container Registry&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/container_registry&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;model_registry&quot;,&quot;title&quot;:&quot;Model registry&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/ml/models&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;operations_menu&quot;,&quot;title&quot;:&quot;Operate&quot;,&quot;icon&quot;:&quot;cloud-pod&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/environments&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;environments&quot;,&quot;title&quot;:&quot;Environments&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/environments&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-environments&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;kubernetes&quot;,&quot;title&quot;:&quot;Kubernetes clusters&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/clusters&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-kubernetes&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;terraform_states&quot;,&quot;title&quot;:&quot;Terraform states&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/terraform&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;infrastructure_registry&quot;,&quot;title&quot;:&quot;Terraform modules&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/terraform_module_registry&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;monitor_menu&quot;,&quot;title&quot;:&quot;Monitor&quot;,&quot;icon&quot;:&quot;monitor&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/error_tracking&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;error_tracking&quot;,&quot;title&quot;:&quot;Error Tracking&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/error_tracking&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;alert_management&quot;,&quot;title&quot;:&quot;Alerts&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/alert_management&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;incidents&quot;,&quot;title&quot;:&quot;Incidents&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/incidents&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false}],&quot;separated&quot;:false},{&quot;id&quot;:&quot;analyze_menu&quot;,&quot;title&quot;:&quot;Analyze&quot;,&quot;icon&quot;:&quot;chart&quot;,&quot;avatar&quot;:null,&quot;avatar_shape&quot;:&quot;rect&quot;,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/value_stream_analytics&quot;,&quot;is_active&quot;:false,&quot;pill_count&quot;:null,&quot;items&quot;:[{&quot;id&quot;:&quot;cycle_analytics&quot;,&quot;title&quot;:&quot;Value stream analytics&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/value_stream_analytics&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-project-cycle-analytics&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;contributors&quot;,&quot;title&quot;:&quot;Contributor analytics&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/graphs/pavlin_yolov10_v11&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;ci_cd_analytics&quot;,&quot;title&quot;:&quot;CI/CD analytics&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/pipelines/charts&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;repository_analytics&quot;,&quot;title&quot;:&quot;Repository analytics&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/graphs/pavlin_yolov10_v11/charts&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:&quot;shortcuts-repository-charts&quot;,&quot;is_active&quot;:false},{&quot;id&quot;:&quot;model_experiments&quot;,&quot;title&quot;:&quot;Model experiments&quot;,&quot;icon&quot;:null,&quot;avatar&quot;:null,&quot;entity_id&quot;:null,&quot;link&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/ml/experiments&quot;,&quot;pill_count&quot;:null,&quot;link_classes&quot;:null,&quot;is_active&quot;:false}],&quot;separated&quot;:false}],&quot;current_context_header&quot;:&quot;Project&quot;,&quot;support_path&quot;:&quot;https://about.gitlab.com/get-help/&quot;,&quot;docs_path&quot;:&quot;/help/docs&quot;,&quot;display_whats_new&quot;:true,&quot;show_version_check&quot;:false,&quot;search&quot;:{&quot;search_path&quot;:&quot;/search&quot;,&quot;issues_path&quot;:&quot;/dashboard/issues&quot;,&quot;mr_path&quot;:&quot;/dashboard/merge_requests&quot;,&quot;autocomplete_path&quot;:&quot;/search/autocomplete&quot;,&quot;settings_path&quot;:&quot;/search/settings&quot;,&quot;search_context&quot;:{&quot;group&quot;:{&quot;id&quot;:618,&quot;name&quot;:&quot;AI Drone&quot;,&quot;full_name&quot;:&quot;AI / Lab / AI Drone&quot;},&quot;group_metadata&quot;:{&quot;issues_path&quot;:&quot;/groups/ai/lab/ai_drone/-/issues&quot;,&quot;mr_path&quot;:&quot;/groups/ai/lab/ai_drone/-/merge_requests&quot;},&quot;project&quot;:{&quot;id&quot;:524,&quot;name&quot;:&quot;Nvidia Jetson&quot;},&quot;project_metadata&quot;:{&quot;mr_path&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/merge_requests&quot;,&quot;issues_path&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/issues&quot;},&quot;code_search&quot;:true,&quot;ref&quot;:&quot;pavlin_yolov10_v11&quot;,&quot;scope&quot;:null,&quot;for_snippets&quot;:null}},&quot;panel_type&quot;:&quot;project&quot;,&quot;shortcut_links&quot;:[{&quot;title&quot;:&quot;Milestones&quot;,&quot;href&quot;:&quot;/dashboard/milestones&quot;,&quot;css_class&quot;:&quot;dashboard-shortcuts-milestones&quot;},{&quot;title&quot;:&quot;Snippets&quot;,&quot;href&quot;:&quot;/dashboard/snippets&quot;,&quot;css_class&quot;:&quot;dashboard-shortcuts-snippets&quot;},{&quot;title&quot;:&quot;Activity&quot;,&quot;href&quot;:&quot;/dashboard/activity&quot;,&quot;css_class&quot;:&quot;dashboard-shortcuts-activity&quot;},{&quot;title&quot;:&quot;Groups&quot;,&quot;href&quot;:&quot;/dashboard/groups&quot;,&quot;css_class&quot;:&quot;dashboard-shortcuts-groups&quot;},{&quot;title&quot;:&quot;Projects&quot;,&quot;href&quot;:&quot;/dashboard/projects&quot;,&quot;css_class&quot;:&quot;dashboard-shortcuts-projects&quot;},{&quot;title&quot;:&quot;Create a new issue&quot;,&quot;href&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/issues/new&quot;,&quot;css_class&quot;:&quot;shortcuts-new-issue&quot;}],&quot;terms&quot;:null,&quot;is_admin&quot;:false,&quot;name&quot;:&quot;Pavlin Penev&quot;,&quot;username&quot;:&quot;ppenev&quot;,&quot;admin_url&quot;:&quot;https://gitlab.od.atncorp.com/admin&quot;,&quot;admin_mode&quot;:{&quot;admin_mode_feature_enabled&quot;:false,&quot;admin_mode_active&quot;:false,&quot;enter_admin_mode_url&quot;:&quot;/admin/session/new&quot;,&quot;leave_admin_mode_url&quot;:&quot;/admin/session/destroy&quot;,&quot;user_is_admin&quot;:false},&quot;avatar_url&quot;:null,&quot;has_link_to_profile&quot;:true,&quot;link_to_profile&quot;:&quot;/ppenev&quot;,&quot;logo_url&quot;:null,&quot;status&quot;:{&quot;can_update&quot;:true,&quot;busy&quot;:null,&quot;customized&quot;:null,&quot;availability&quot;:&quot;&quot;,&quot;emoji&quot;:null,&quot;message_html&quot;:null,&quot;message&quot;:null,&quot;clear_after&quot;:null},&quot;settings&quot;:{&quot;has_settings&quot;:true,&quot;profile_path&quot;:&quot;/-/user_settings/profile&quot;,&quot;profile_preferences_path&quot;:&quot;/-/profile/preferences&quot;},&quot;user_counts&quot;:{&quot;assigned_issues&quot;:0,&quot;assigned_merge_requests&quot;:0,&quot;review_requested_merge_requests&quot;:0,&quot;todos&quot;:0,&quot;last_update&quot;:1729159598237},&quot;can_sign_out&quot;:true,&quot;sign_out_link&quot;:&quot;/users/sign_out&quot;,&quot;issues_dashboard_path&quot;:&quot;/dashboard/issues?assignee_username=ppenev&quot;,&quot;merge_request_dashboard_path&quot;:null,&quot;todos_dashboard_path&quot;:&quot;/dashboard/todos&quot;,&quot;create_new_menu_groups&quot;:[{&quot;name&quot;:&quot;In this project&quot;,&quot;items&quot;:[{&quot;text&quot;:&quot;New issue&quot;,&quot;href&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/issues/new&quot;,&quot;component&quot;:null,&quot;extraAttrs&quot;:{&quot;data-track-label&quot;:&quot;new_issue&quot;,&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-property&quot;:&quot;nav_create_menu&quot;,&quot;data-testid&quot;:&quot;create_menu_item&quot;,&quot;data-qa-create-menu-item&quot;:&quot;new_issue&quot;}},{&quot;text&quot;:&quot;New merge request&quot;,&quot;href&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/merge_requests/new&quot;,&quot;component&quot;:null,&quot;extraAttrs&quot;:{&quot;data-track-label&quot;:&quot;new_mr&quot;,&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-property&quot;:&quot;nav_create_menu&quot;,&quot;data-testid&quot;:&quot;create_menu_item&quot;,&quot;data-qa-create-menu-item&quot;:&quot;new_mr&quot;}},{&quot;text&quot;:&quot;New snippet&quot;,&quot;href&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/snippets/new&quot;,&quot;component&quot;:null,&quot;extraAttrs&quot;:{&quot;data-track-label&quot;:&quot;new_snippet&quot;,&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-property&quot;:&quot;nav_create_menu&quot;,&quot;data-testid&quot;:&quot;create_menu_item&quot;,&quot;data-qa-create-menu-item&quot;:&quot;new_snippet&quot;}}]},{&quot;name&quot;:&quot;In GitLab&quot;,&quot;items&quot;:[{&quot;text&quot;:&quot;New project/repository&quot;,&quot;href&quot;:&quot;/projects/new&quot;,&quot;component&quot;:null,&quot;extraAttrs&quot;:{&quot;data-track-label&quot;:&quot;general_new_project&quot;,&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-property&quot;:&quot;nav_create_menu&quot;,&quot;data-testid&quot;:&quot;create_menu_item&quot;,&quot;data-qa-create-menu-item&quot;:&quot;general_new_project&quot;}},{&quot;text&quot;:&quot;New group&quot;,&quot;href&quot;:&quot;/groups/new&quot;,&quot;component&quot;:null,&quot;extraAttrs&quot;:{&quot;data-track-label&quot;:&quot;general_new_group&quot;,&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-property&quot;:&quot;nav_create_menu&quot;,&quot;data-testid&quot;:&quot;create_menu_item&quot;,&quot;data-qa-create-menu-item&quot;:&quot;general_new_group&quot;}},{&quot;text&quot;:&quot;New snippet&quot;,&quot;href&quot;:&quot;/-/snippets/new&quot;,&quot;component&quot;:null,&quot;extraAttrs&quot;:{&quot;data-track-label&quot;:&quot;general_new_snippet&quot;,&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-property&quot;:&quot;nav_create_menu&quot;,&quot;data-testid&quot;:&quot;create_menu_item&quot;,&quot;data-qa-create-menu-item&quot;:&quot;general_new_snippet&quot;}}]}],&quot;merge_request_menu&quot;:[{&quot;name&quot;:&quot;Merge requests&quot;,&quot;items&quot;:[{&quot;text&quot;:&quot;Assigned&quot;,&quot;href&quot;:&quot;/dashboard/merge_requests?assignee_username=ppenev&quot;,&quot;count&quot;:0,&quot;userCount&quot;:&quot;assigned_merge_requests&quot;,&quot;extraAttrs&quot;:{&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-label&quot;:&quot;merge_requests_assigned&quot;,&quot;data-track-property&quot;:&quot;nav_core_menu&quot;,&quot;class&quot;:&quot;dashboard-shortcuts-merge_requests&quot;}},{&quot;text&quot;:&quot;Review requests&quot;,&quot;href&quot;:&quot;/dashboard/merge_requests?reviewer_username=ppenev&quot;,&quot;count&quot;:0,&quot;userCount&quot;:&quot;review_requested_merge_requests&quot;,&quot;extraAttrs&quot;:{&quot;data-track-action&quot;:&quot;click_link&quot;,&quot;data-track-label&quot;:&quot;merge_requests_to_review&quot;,&quot;data-track-property&quot;:&quot;nav_core_menu&quot;,&quot;class&quot;:&quot;dashboard-shortcuts-review_requests&quot;}}]}],&quot;projects_path&quot;:&quot;/dashboard/projects&quot;,&quot;groups_path&quot;:&quot;/dashboard/groups&quot;,&quot;gitlab_com_but_not_canary&quot;:false,&quot;gitlab_com_and_canary&quot;:false,&quot;canary_toggle_com_url&quot;:&quot;https://next.gitlab.com&quot;,&quot;current_context&quot;:{&quot;namespace&quot;:&quot;projects&quot;,&quot;item&quot;:{&quot;id&quot;:524,&quot;name&quot;:&quot;Nvidia Jetson&quot;,&quot;namespace&quot;:&quot;AI / Lab / AI Drone / Nvidia Jetson&quot;,&quot;webUrl&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson&quot;,&quot;avatarUrl&quot;:null}},&quot;pinned_items&quot;:[&quot;project_issue_list&quot;,&quot;project_merge_request_list&quot;],&quot;update_pins_url&quot;:&quot;/-/users/pins&quot;,&quot;is_impersonating&quot;:false,&quot;stop_impersonation_path&quot;:&quot;/admin/impersonation&quot;,&quot;track_visits_path&quot;:&quot;/-/track_namespace_visits&quot;,&quot;work_items&quot;:null}"></aside>

<div class="content-wrapper">

<div class="broadcast-wrapper">




</div>
<div class="alert-wrapper gl-flex gl-flex-col gl-gap-3 container-fluid container-limited">
























<div class="flash-container flash-container-page sticky" data-testid="flash-container">
<div id="js-global-alerts"></div>
</div>


</div>
<div class="top-bar-fixed container-fluid" data-testid="top-bar">
<div class="top-bar-container gl-flex gl-items-center gl-gap-2">
<button class="gl-button btn btn-icon btn-md btn-default btn-default-tertiary js-super-sidebar-toggle-expand super-sidebar-toggle -gl-ml-3" aria-controls="super-sidebar" aria-expanded="false" aria-label="Primary navigation sidebar" type="button"><svg class="s16 gl-icon gl-button-icon " data-testid="sidebar-icon"><use href="/assets/icons-50888ef7fb46c3a1fb53bc67cfc1085be59395f0d49dd55cdd8a8e269dede05b.svg#sidebar"></use></svg>

</button>
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"BreadcrumbList","itemListElement":[{"@type":"ListItem","position":1,"name":"AI","item":"https://gitlab.od.atncorp.com/ai"},{"@type":"ListItem","position":2,"name":"Lab","item":"https://gitlab.od.atncorp.com/ai/lab"},{"@type":"ListItem","position":3,"name":"AI Drone","item":"https://gitlab.od.atncorp.com/ai/lab/ai_drone"},{"@type":"ListItem","position":4,"name":"Nvidia Jetson","item":"https://gitlab.od.atncorp.com/ai/lab/ai_drone/nvidia-jetson"},{"@type":"ListItem","position":5,"name":"Repository","item":"https://gitlab.od.atncorp.com/ai/lab/ai_drone/nvidia-jetson/-/blob/pavlin_yolov10_v11/docker/README.md"}]}


</script>
<div data-testid="breadcrumb-links" id="js-vue-page-breadcrumbs-wrapper">
<div data-breadcrumbs-json="[{&quot;text&quot;:&quot;AI&quot;,&quot;href&quot;:&quot;/ai&quot;,&quot;avatarPath&quot;:null},{&quot;text&quot;:&quot;Lab&quot;,&quot;href&quot;:&quot;/ai/lab&quot;,&quot;avatarPath&quot;:null},{&quot;text&quot;:&quot;AI Drone&quot;,&quot;href&quot;:&quot;/ai/lab/ai_drone&quot;,&quot;avatarPath&quot;:null},{&quot;text&quot;:&quot;Nvidia Jetson&quot;,&quot;href&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson&quot;,&quot;avatarPath&quot;:null},{&quot;text&quot;:&quot;Repository&quot;,&quot;href&quot;:&quot;/ai/lab/ai_drone/nvidia-jetson/-/blob/pavlin_yolov10_v11/docker/README.md&quot;,&quot;avatarPath&quot;:null}]" id="js-vue-page-breadcrumbs"></div>
<div id="js-injected-page-breadcrumbs"></div>
</div>


<div id="js-work-item-feedback"></div>


</div>
</div>

<div class="container-fluid container-limited project-highlight-puc">
<main class="content" id="content-body" itemscope itemtype="http://schema.org/SoftwareSourceCode">




<div class="js-signature-container" data-signatures-path="/ai/lab/ai_drone/nvidia-jetson/-/commits/a07eda24c0df9617c0974b482b1bc3edbc8072fd/signatures?limit=1"></div>
<div class="gl-alert gl-mt-3 gl-alert-success" role="alert">
<div class="gl-alert-icon-container">
<svg class="s16 gl-alert-icon gl-alert-icon-no-title" data-testid="check-circle-icon"><use href="/assets/icons-50888ef7fb46c3a1fb53bc67cfc1085be59395f0d49dd55cdd8a8e269dede05b.svg#check-circle"></use></svg>
</div>
<button class="gl-button btn btn-icon btn-sm btn-default btn-default-tertiary js-close gl-dismiss-btn js-close-banner" aria-label="Dismiss" type="button"><svg class="s16 gl-icon gl-button-icon " data-testid="close-icon"><use href="/assets/icons-50888ef7fb46c3a1fb53bc67cfc1085be59395f0d49dd55cdd8a8e269dede05b.svg#close"></use></svg>

</button>
<div class="gl-alert-content" role="alert">
<div class="gl-alert-body">
<span>You pushed to</span>
<strong class="gl-inline-flex gl-max-w-1/2" data-toggle="tooltip" title="pavlin_yolov10_v11">
<a class="ref-name gl-truncate" href="/ai/lab/ai_drone/nvidia-jetson/-/commits/pavlin_yolov10_v11">pavlin_yolov10_v11</a>
</strong>
<time class="js-timeago" title="Oct 17, 2024 10:05am" datetime="2024-10-17T10:05:02Z" data-toggle="tooltip" data-placement="top" data-container="body">Oct 17, 2024</time>

</div>
<div class="gl-alert-actions">
<a data-testid="create-merge-request-button" class="gl-button btn btn-md btn-confirm " href="/ai/lab/ai_drone/nvidia-jetson/-/merge_requests/new?merge_request%5Bsource_branch%5D=pavlin_yolov10_v11"><span class="gl-button-text">
Create merge request

</span>

</a>
</div>
</div>
</div>

<div class="tree-holder gl-pt-4" id="tree-holder">
<div class="nav-block">
<div class="tree-ref-container">
<div class="tree-ref-holder gl-max-w-26">
<div data-project-id="524" data-project-root-path="/ai/lab/ai_drone/nvidia-jetson" data-ref="pavlin_yolov10_v11" data-ref-type="" id="js-tree-ref-switcher"></div>
</div>
<ul class="breadcrumb repo-breadcrumb">
<li class="breadcrumb-item">
<a href="/ai/lab/ai_drone/nvidia-jetson/-/tree/pavlin_yolov10_v11">nvidia-jetson
</a></li>
<li class="breadcrumb-item">
<a href="/ai/lab/ai_drone/nvidia-jetson/-/tree/pavlin_yolov10_v11/docker">docker</a>
</li>
<li class="breadcrumb-item">
<a href="/ai/lab/ai_drone/nvidia-jetson/-/blob/pavlin_yolov10_v11/docker/README.md"><strong>README.md</strong>
</a></li>
</ul>
</div>
<div class="tree-controls gl-flex gl-flex-wrap sm:gl-flex-nowrap gl-items-baseline gl-gap-3">
<button class="gl-button btn btn-md btn-default has-tooltip shortcuts-find-file" title="Go to file, press &lt;kbd class=&#39;flat ml-1&#39; aria-hidden=true&gt;/~&lt;/kbd&gt; or &lt;kbd class=&#39;flat ml-1&#39; aria-hidden=true&gt;t&lt;/kbd&gt;" aria-keyshortcuts="/+~ t" data-html="true" data-event-tracking="click_find_file_button_on_repository_pages" type="button"><span class="gl-button-text">
Find file

</span>

</button>
<a data-event-tracking="click_blame_control_on_blob_page" class="gl-button btn btn-md btn-default js-blob-blame-link" href="/ai/lab/ai_drone/nvidia-jetson/-/blame/pavlin_yolov10_v11/docker/README.md"><span class="gl-button-text">
Blame
</span>

</a>
<a data-event-tracking="click_history_control_on_blob_page" class="gl-button btn btn-md btn-default " href="/ai/lab/ai_drone/nvidia-jetson/-/commits/pavlin_yolov10_v11/docker/README.md"><span class="gl-button-text">
History
</span>

</a>
<a aria-keyshortcuts="y" class="gl-button btn btn-md btn-default has-tooltip js-data-file-blob-permalink-url" data-html="true" title="Go to permalink &lt;kbd class=&#39;flat ml-1&#39; aria-hidden=true&gt;y&lt;/kbd&gt;" href="/ai/lab/ai_drone/nvidia-jetson/-/blob/a07eda24c0df9617c0974b482b1bc3edbc8072fd/docker/README.md"><span class="gl-button-text">
Permalink
</span>

</a>
</div>
</div>

<div class="info-well gl-hidden sm:gl-block">
<div class="well-segment">
<ul class="blob-commit-info">
<li class="commit flex-row js-toggle-container" id="commit-a07eda24">
<div class="avatar-cell gl-hidden sm:gl-block">
<a href="/ppenev"><img alt="Pavlin Penev&#39;s avatar" src="/assets/no_avatar-849f9c04a3a0d0cea2424ae97b27447dc64a7dbfae83c036c45b403392f0e8ba.png" class="avatar s40 gl-hidden sm:gl-inline-block" title="Pavlin Penev"></a>
</div>
<div class="commit-detail flex-list gl-flex gl-justify-between gl-items-center gl-grow gl-min-w-0">
<div class="commit-content" data-testid="commit-content">
<a class="commit-row-message item-title js-onboarding-commit-item " href="/ai/lab/ai_drone/nvidia-jetson/-/commit/a07eda24c0df9617c0974b482b1bc3edbc8072fd">Update file README.md</a>
<span class="commit-row-message d-inline d-sm-none">
&middot;
a07eda24
</span>
<div class="committer">
<a class="commit-author-link js-user-link" data-user-id="109" href="/ppenev">Pavlin Penev</a> authored <time class="js-timeago" title="Oct 17, 2024 10:05am" datetime="2024-10-17T10:05:01Z" data-toggle="tooltip" data-placement="bottom" data-container="body">Oct 17, 2024</time>
</div>

</div>
<div class="commit-actions flex-row">

<div class="js-commit-pipeline-status" data-endpoint="/ai/lab/ai_drone/nvidia-jetson/-/commit/a07eda24c0df9617c0974b482b1bc3edbc8072fd/pipelines?ref=pavlin_yolov10_v11"></div>
<div class="commit-sha-group btn-group gl-hidden sm:gl-flex">
<div class="label label-monospace monospace">
a07eda24
</div>
<button class="gl-button btn btn-icon btn-md btn-default " title="Copy commit SHA" aria-label="Copy commit SHA" aria-live="polite" data-toggle="tooltip" data-placement="bottom" data-container="body" data-html="true" data-category="primary" data-size="medium" data-clipboard-text="a07eda24c0df9617c0974b482b1bc3edbc8072fd" type="button"><svg class="s16 gl-icon gl-button-icon " data-testid="copy-to-clipboard-icon"><use href="/assets/icons-50888ef7fb46c3a1fb53bc67cfc1085be59395f0d49dd55cdd8a8e269dede05b.svg#copy-to-clipboard"></use></svg>

</button>

</div>
</div>
</div>
</li>

</ul>
</div>

</div>
<div class="blob-content-holder js-per-page" data-blame-per-page="1000" id="blob-content-holder">
<div data-blob-path="docker/README.md" data-can-download-code="true" data-original-branch="pavlin_yolov10_v11" data-project-path="ai/lab/ai_drone/nvidia-jetson" data-ref-type="" data-resource-id="gid://gitlab/Project/524" data-target-branch="pavlin_yolov10_v11" data-user-id="gid://gitlab/User/109" id="js-view-blob-app">
<div class="gl-spinner-container" role="status"><span aria-label="Loading" class="gl-spinner gl-spinner-md gl-spinner-dark !gl-align-text-bottom"></span></div>
</div>
</div>

</div>
<script>
//<![CDATA[
  window.gl = window.gl || {};
  window.gl.webIDEPath = '/-/ide/project/ai/lab/ai_drone/nvidia-jetson/edit/pavlin_yolov10_v11/-/docker/README.md'


//]]>
</script>
<div data-ambiguous="false" data-ref="pavlin_yolov10_v11" id="js-ambiguous-ref-modal"></div>

</main>
</div>


</div>
</div>


<script>
//<![CDATA[
if ('loading' in HTMLImageElement.prototype) {
  document.querySelectorAll('img.lazy').forEach(img => {
    img.loading = 'lazy';
    let imgUrl = img.dataset.src;
    // Only adding width + height for avatars for now
    if (imgUrl.indexOf('/avatar/') > -1 && imgUrl.indexOf('?') === -1) {
      const targetWidth = img.getAttribute('width') || img.width;
      imgUrl += `?width=${targetWidth}`;
    }
    img.src = imgUrl;
    img.removeAttribute('data-src');
    img.classList.remove('lazy');
    img.classList.add('js-lazy-loaded');
    img.dataset.testid = 'js-lazy-loaded-content';
  });
}

//]]>
</script>
<script>
//<![CDATA[
gl = window.gl || {};
gl.experiments = {};


//]]>
</script>

</body>
</html>

