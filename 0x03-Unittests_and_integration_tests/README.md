<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <meta name="description" content="">
    <meta name="google" content="notranslate">

      <script>
    window.dataLayer = window.dataLayer || [];
    dataLayer.push({"userId":220204,"visitorType":"student","batch":{"id":58,"fullNameWithC":"LOS-1122 (C#11)","schoolLocation":{"id":3,"name":"Lagos"}},"curriculum":{"id":17,"name":"Short Specializations"}});

    window.gtm_user_custom_event = function (name, options) {
      if (typeof name === 'undefined') {
        return;
      }

      window.dataLayer.push({
        customEventOptions: typeof options !== 'undefined' ? options : {},
        event: name,
      });
    }
  </script>

  <!-- Google Tag Manager -->
  <script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
  new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
  j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
  'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
  })(window,document,'script','dataLayer','GTM-N4C8MF2');</script>
  <!-- End Google Tag Manager -->


    <title>Project: 0x03. Unittests and Integration Tests | Lagos Intranet</title>

      <link rel="stylesheet" href="https://use.typekit.net/xgz4ilr.css">
      <link rel="stylesheet" media="all" href="/assets/application_alx-c08b05e2a2a9e57e45bb68c10a121418973533958ae33cebc0fe085102206dcf.css" />
      <script src="https://www.gstatic.com/charts/loader.js"></script>
      <script src="/assets/application-42065a47b2e3f8e2163cd65e151b8e28ed161d3cab1676f66507ee99bbc907e6.js"></script>
      <link rel="shortcut icon" type="image/x-icon" href="/favicon_alx.ico" />
      <meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="WhQ2ErfG5VTxZRGzLkfEpDVDrquKxlBGYp-Ln1Fc6N-rrPSjmS5pwLLHJBi64NsqO1pACFxiEKVNX45-nc3rlw" />

      <link rel="apple-touch-icon" href="/apple-touch-icon_alx.png">

      <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
      <!--[if lt IE 9]>
        <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
        <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
      <![endif]-->

      <!-- Store user timezone -->
      <script>
        Cookies.set('timezone', (new Date()).getTimezoneOffset() / -60.0);
      </script>

      <!-- intro.js for interactive onboarding -->

      <!-- React -->
      <script src="/packs/js/application-18c31b7f5878da16cd3a.js"></script>
      <link rel="stylesheet" media="screen" href="/packs/css/application-87456da7.css" />
  </head>

  <body class="signed_in env_production notranslate"
        translate="no"
        class="notranslate"
        data-theme-suffix="_alx">
      <!-- Google Tag Manager (noscript) -->
  <noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-N4C8MF2"
  height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
  <!-- End Google Tag Manager (noscript) -->


      <input type="hidden" id="hbtn-slack-url" value="https://alx-students.slack.com">
      <nav class="navbar navbar-default navbar-fixed-top topbar visible-xs">
  <div class="navbar-header">
    <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar-mobile" aria-expanded="false">
      <span class="sr-only">Toggle navigation</span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
      <span class="icon-bar"></span>
    </button>

    <a class="navbar-brand" href="/">
      <div class="logo"></div>
</a>  </div>

  <div class="collapse navbar-collapse navigation" id="navbar-mobile">
    <ul class="nav navbar-nav">
      


    <li data-container="body" data-placement="right" data-toggle="tooltip" title="My Planning"><a href="/planning/me"><div class="icon "><i aria-hidden="true" class="fa-solid fa-calendar "></i></div><div class="visible-xs">My Planning</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-current-projects-item" title="Projects"><a href="/projects/current"><div class="icon "><i aria-hidden="true" class="fa-solid fa-code-fork "></i></div><div class="visible-xs">Projects</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="QA Reviews I can make"><a href="/corrections/to_review"><div class="icon "><i aria-hidden="true" class="fa-solid fa-check "></i></div><div class="visible-xs">QA Reviews I can make</div></a></li>
    
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Evaluation quizzes"><a href="/dashboards/my_current_evaluation_quizzes"><div class="icon "><i aria-hidden="true" class="fa-solid fa-question "></i></div><div class="visible-xs">Evaluation quizzes</div></a></li>

    <hr title="My resources">

    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Curriculums"><a href="/dashboards/my_curriculums"><div class="icon "><i aria-hidden="true" class="fa-solid fa-graduation-cap "></i></div><div class="visible-xs">Curriculums</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-concepts-item" title="Concepts"><a href="/concepts"><div class="icon "><i aria-hidden="true" class="fa-solid fa-file-text "></i></div><div class="visible-xs">Concepts</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-video-rooms" title="Conference rooms"><a href="/dashboards/video_rooms"><div class="icon "><i aria-hidden="true" class="fa-solid fa-comments "></i></div><div class="visible-xs">Conference rooms</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Servers"><a href="/servers"><div class="icon "><i aria-hidden="true" class="fa-solid fa-server "></i></div><div class="visible-xs">Servers</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-my-containers" title="Sandboxes"><a href="/user_containers/current"><div class="icon "><i aria-hidden="true" class="fa-solid fa-terminal "></i></div><div class="visible-xs">Sandboxes</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Tools"><a href="/dashboards/my_tools"><div class="icon "><i aria-hidden="true" class="fa-solid fa-wrench "></i></div><div class="visible-xs">Tools</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Video on demand"><a href="/dashboards/videos"><div class="icon "><i aria-hidden="true" class="fa-solid fa-film "></i></div><div class="visible-xs">Video on demand</div></a></li>

      <hr title="My campus">

      
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Peers"><a href="/users/peers"><div class="icon "><i aria-hidden="true" class="fa-solid fa-users "></i></div><div class="visible-xs">Peers</div></a></li>
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Captain&#39;s Logs"><a href="/dashboards/my_captain_log"><div class="icon "><i aria-hidden="true" class="fa-solid fa-book "></i></div><div class="visible-xs">Captain&#39;s Logs</div></a></li>


<hr class="visible-xs">

<li>

      <div
      data-container="body"
      data-placement="right"
      data-toggle="tooltip"
      title="Discord">
        <a rel="noreferrer" target="_blank" href="https://discord.com/app">
          <div class="icon discord">
            <i aria-hidden="true" class="fa-brands fa-discord "></i>
          </div>
          <div class="visible-xs">Discord</div>
</a>      </div>

  <div
    data-container="body"
    data-placement="right"
    data-toggle="tooltip"
    title="My Profile">
    <a href="/users/my_profile">
        <div class="image ">
          <div class="inner" style="background-image: url('https://s3.amazonaws.com/alx-intranet.hbtn.io/users/photos/000/220/204/thumb/esther.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231108%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20231108T051821Z&amp;X-Amz-Expires=600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=feadf4811cf2f4ad99aa805f0bf36d1667bfd10047a0ccc78f4e403e5364caa4')"></div>
        </div>

      <div class="visible-xs">My Profile</div>
</a>  </div>
</li>


    </ul>
  </div>
</nav>

      <div class="hidden-xs navigation sidebar">
  <a class="logo-container" href="/">
    <div class="logo"></div>
</a>
  <ul>
    


    <li data-container="body" data-placement="right" data-toggle="tooltip" title="My Planning"><a href="/planning/me"><div class="icon "><i aria-hidden="true" class="fa-solid fa-calendar "></i></div><div class="visible-xs">My Planning</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-current-projects-item" title="Projects"><a href="/projects/current"><div class="icon "><i aria-hidden="true" class="fa-solid fa-code-fork "></i></div><div class="visible-xs">Projects</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="QA Reviews I can make"><a href="/corrections/to_review"><div class="icon "><i aria-hidden="true" class="fa-solid fa-check "></i></div><div class="visible-xs">QA Reviews I can make</div></a></li>
    
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Evaluation quizzes"><a href="/dashboards/my_current_evaluation_quizzes"><div class="icon "><i aria-hidden="true" class="fa-solid fa-question "></i></div><div class="visible-xs">Evaluation quizzes</div></a></li>

    <hr title="My resources">

    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Curriculums"><a href="/dashboards/my_curriculums"><div class="icon "><i aria-hidden="true" class="fa-solid fa-graduation-cap "></i></div><div class="visible-xs">Curriculums</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-concepts-item" title="Concepts"><a href="/concepts"><div class="icon "><i aria-hidden="true" class="fa-solid fa-file-text "></i></div><div class="visible-xs">Concepts</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-video-rooms" title="Conference rooms"><a href="/dashboards/video_rooms"><div class="icon "><i aria-hidden="true" class="fa-solid fa-comments "></i></div><div class="visible-xs">Conference rooms</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Servers"><a href="/servers"><div class="icon "><i aria-hidden="true" class="fa-solid fa-server "></i></div><div class="visible-xs">Servers</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" id="sidebar-dashboards-my-containers" title="Sandboxes"><a href="/user_containers/current"><div class="icon "><i aria-hidden="true" class="fa-solid fa-terminal "></i></div><div class="visible-xs">Sandboxes</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Tools"><a href="/dashboards/my_tools"><div class="icon "><i aria-hidden="true" class="fa-solid fa-wrench "></i></div><div class="visible-xs">Tools</div></a></li>
    <li data-container="body" data-placement="right" data-toggle="tooltip" title="Video on demand"><a href="/dashboards/videos"><div class="icon "><i aria-hidden="true" class="fa-solid fa-film "></i></div><div class="visible-xs">Video on demand</div></a></li>

      <hr title="My campus">

      
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Peers"><a href="/users/peers"><div class="icon "><i aria-hidden="true" class="fa-solid fa-users "></i></div><div class="visible-xs">Peers</div></a></li>
      <li data-container="body" data-placement="right" data-toggle="tooltip" title="Captain&#39;s Logs"><a href="/dashboards/my_captain_log"><div class="icon "><i aria-hidden="true" class="fa-solid fa-book "></i></div><div class="visible-xs">Captain&#39;s Logs</div></a></li>


<hr class="visible-xs">

<li>

      <div
      data-container="body"
      data-placement="right"
      data-toggle="tooltip"
      title="Discord">
        <a rel="noreferrer" target="_blank" href="https://discord.com/app">
          <div class="icon discord">
            <i aria-hidden="true" class="fa-brands fa-discord "></i>
          </div>
          <div class="visible-xs">Discord</div>
</a>      </div>

  <div
    data-container="body"
    data-placement="right"
    data-toggle="tooltip"
    title="My Profile">
    <a href="/users/my_profile">
        <div class="image ">
          <div class="inner" style="background-image: url('https://s3.amazonaws.com/alx-intranet.hbtn.io/users/photos/000/220/204/thumb/esther.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231108%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20231108T051821Z&amp;X-Amz-Expires=600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=feadf4811cf2f4ad99aa805f0bf36d1667bfd10047a0ccc78f4e403e5364caa4')"></div>
        </div>

      <div class="visible-xs">My Profile</div>
</a>  </div>
</li>


  </ul>
</div>


    <main>
        <div id="layout-bars">
          
          <div class="px-5 py-3" id="student-switch-curriculum">
  <div class="dropdown d-flex flex-column gap-1">
    <span class="fs-small text-muted">Curriculum</span>

    <div aria-haspopup="true" aria-expanded="false" class="align-items-center d-flex gap-3" data-toggle="dropdown" id="student-switch-curriculum-dropdown" role="button">
      <div class="d-flex flex-column" style="line-height: 16px">
        <span class="fs-4 fw-600">
          Short Specializations
        </span>
        <span class="fs-small text-muted">
          Average: <span class="fw-500">77.57%</span>
        </span>
      </div>

      <div class="d-flex flex-column justify-content-center">
        <span style="margin-bottom: -4px">
          <i aria-hidden="true" class="fa-solid fa-angle-up  fa-fw"></i>
        </span>
        <span style="margin-top: -4px">
          <i aria-hidden="true" class="fa-solid fa-angle-down  fa-fw"></i>
        </span>
      </div>
    </div>

    <ul aria-labelledby="student-switch-curriculum-dropdown" class="dropdown-menu fs-5">
        <li>
          <a href="/curriculums/1/observe">
            <div class="align-items-center d-flex py-2">
              <div class="d-flex flex-column" style="line-height: 16px">
                <span class="fs-4 fw-500">
                  SE Foundations
                </span>
                <span class="text-muted">
                  Average: <span class="fw-500">126.44%</span>
                </span>
              </div>

            </div>
</a>        </li>
        <li>
          <a href="/curriculums/17/observe">
            <div class="align-items-center d-flex py-2">
              <div class="d-flex flex-column" style="line-height: 16px">
                <span class="fs-4 fw-500">
                  Short Specializations
                </span>
                <span class="text-muted">
                  Average: <span class="fw-500">77.57%</span>
                </span>
              </div>

                <span class="fw-600 text-info" style="margin-left: 42px">
                  <i aria-hidden="true" class="fa-solid fa-check "></i>
                </span>
            </div>
</a>        </li>
    </ul>
  </div>
</div>

          
          
          
          
        </div>

      <article class="">

        
<div class="project row">
  <div class="col-xs-12 col-md-10 col-lg-8 contains-images">

      <h1 class="gap">0x03. Unittests and Integration Tests</h1>

  <div data-react-class="tags/Tags" data-react-props="{&quot;tags&quot;:[{&quot;id&quot;:25,&quot;value&quot;:&quot;UnitTests&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;},{&quot;id&quot;:35,&quot;value&quot;:&quot;Back-end&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;},{&quot;id&quot;:60,&quot;value&quot;:&quot;Integration tests&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;}]}" data-react-cache-id="tags/Tags-0"></div>

  <div data-react-class="projects/ProjectMetadata" data-react-props="{&quot;metadata&quot;:{&quot;author&quot;:&quot;Emmanuel Turlay, Staff Software Engineer at Cruise&quot;,&quot;weight&quot;:1,&quot;correction&quot;:{&quot;released&quot;:true,&quot;requires_auto_correction&quot;:true,&quot;requires_manual_correction&quot;:false},&quot;bpi&quot;:{&quot;current&quot;:false,&quot;in_second_deadline&quot;:false,&quot;starts_at&quot;:&quot;2023-10-26T06:00:00.000+01:00&quot;,&quot;ends_at&quot;:&quot;2023-10-31T06:00:00.000+01:00&quot;,&quot;second_deadline_at&quot;:&quot;2023-11-04T06:00:00.000+01:00&quot;}}}" data-react-cache-id="projects/ProjectMetadata-0"></div>

  <div class="sm-gap clean well">
  <h4>In a nutshell&hellip;</h4>
  <ul>


      <li>
        <strong>Auto QA review:</strong>
          0.0/26 mandatory
            &
            0.0/4 optional
      </li>
    <li>
      <strong>Altogether:</strong>
        &nbsp;<strong>0.0%</strong>
        <ul>
          <li>Mandatory: 0.0%</li>
            <li>Optional: 0.0%</li>
            <li>
              Calculation:&nbsp;
                  0.0%
                    + (0.0% * 0.0%)
              &nbsp;==&nbsp;<strong>0.0%</strong>
            </li>
        </ul>
    </li>
  </ul>

</div>




    


    <div id="project_id" style="display: none" data-project-id="1237"></div>



      

      

      <div class="panel panel-default" id="project-description">
  <div class="panel-body">
    <p><img src="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/1/f088970b450e82c881ea.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231108%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231108T051821Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6cb24aa26c7fea6756404587bc18afbfbd5ae36f6cae486dbc24e6b2033d34ea" alt="" loading='lazy' style="" /></p>

<p>Unit testing is the process of testing that a particular function returns expected results
for different set of inputs. A unit test is supposed to test standard inputs and corner cases. A unit test should only test the logic defined inside the tested function. Most calls to additional functions should be mocked, especially if they make network or database calls.</p>

<p>The goal of a unit test is to answer the question: if everything defined outside this function works as expected, does this function work as expected?</p>

<p>Integration tests aim to test a code path end-to-end. In general, only low level functions that make external calls such as HTTP requests, file I/O, database I/O, etc. are mocked.</p>

<p>Integration tests will test interactions between every part of your code.</p>

<p>Execute your tests with </p>

<pre><code class="bash">$ python -m unittest path/to/test_file.py
</code></pre>

<h2>Resources</h2>

<p><strong>Read or watch:</strong></p>

<ul>
<li><a href="/rltoken/a_AEObGK8jeqPtTPmm-gIA" title="unittest — Unit testing framework" target="_blank">unittest — Unit testing framework</a></li>
<li><a href="/rltoken/PKetnACd7FfRiU8_kpe5EA" title="unittest.mock — mock object library" target="_blank">unittest.mock — mock object library</a></li>
<li><a href="/rltoken/2ueVPK1kWZuz525FvZ1v2Q" title="How to mock a readonly property with mock?" target="_blank">How to mock a readonly property with mock?</a></li>
<li><a href="/rltoken/mI7qc3Y42aZ7GTlLXDxgEg" title="parameterized" target="_blank">parameterized</a></li>
<li><a href="/rltoken/x83Hdr54q4Vax5xQ2Z3HSA" title="Memoization" target="_blank">Memoization</a></li>
</ul>

<h2>Learning Objectives</h2>

<p>At the end of this project, you are expected to be able to <a href="/rltoken/NfT-nNKrNHGrDMY-Qm-1Dg" title="explain to anyone" target="_blank">explain to anyone</a>, <strong>without the help of Google</strong>:</p>

<ul>
<li>The difference between unit and integration tests.</li>
<li>Common testing patterns such as mocking, parametrizations and fixtures</li>
</ul>

<h2>Requirements</h2>

<ul>
<li>All your files will be interpreted/compiled on Ubuntu 18.04 LTS using <code>python3</code> (version 3.7)</li>
<li>All your files should end with a new line</li>
<li>The first line of all your files should be exactly <code>#!/usr/bin/env python3</code></li>
<li>A <code>README.md</code> file, at the root of the folder of the project, is mandatory</li>
<li>Your code should use the <code>pycodestyle</code> style (version 2.5)</li>
<li>All your files must be executable</li>
<li>All your modules should have a documentation (<code>python3 -c &#39;print(__import__(&quot;my_module&quot;).__doc__)&#39;</code>)</li>
<li>All your classes should have a documentation (<code>python3 -c &#39;print(__import__(&quot;my_module&quot;).MyClass.__doc__)&#39;</code>)</li>
<li>All your functions (inside and outside a class) should have a documentation (<code>python3 -c &#39;print(__import__(&quot;my_module&quot;).my_function.__doc__)&#39;</code> and <code>python3 -c &#39;print(__import__(&quot;my_module&quot;).MyClass.my_function.__doc__)&#39;</code>)</li>
<li>A documentation is not a simple word, it&rsquo;s a real sentence explaining what&rsquo;s the purpose of the module, class or method (the length of it will be verified)</li>
<li>All your functions and coroutines must be type-annotated.</li>
</ul>

<h2>Required Files</h2>

<h3><code>utils.py</code> (or <a href="https://intranet-projects-files.s3.amazonaws.com/webstack/utils.py" title="download" target="_blank">download</a>)</h3>

<details>
<summary>Click to show/hide file contents</summary>
<pre>
<code>
#!/usr/bin/env python3
"""Generic utilities for github org client.
"""
import requests
from functools import wraps
from typing import (
    Mapping,
    Sequence,
    Any,
    Dict,
    Callable,
)

__all__ = [
    "access_nested_map",
    "get_json",
    "memoize",
]


def access_nested_map(nested_map: Mapping, path: Sequence) -> Any:
    """Access nested map with key path.
    Parameters
    ----------
    nested_map: Mapping
        A nested map
    path: Sequence
        a sequence of key representing a path to the value
    Example
    -------
    >>> nested_map = {"a": {"b": {"c": 1}}}
    >>> access_nested_map(nested_map, ["a", "b", "c"])
    1
    """
    for key in path:
        if not isinstance(nested_map, Mapping):
            raise KeyError(key)
        nested_map = nested_map[key]

    return nested_map


def get_json(url: str) -> Dict:
    """Get JSON from remote URL.
    """
    response = requests.get(url)
    return response.json()


def memoize(fn: Callable) -> Callable:
    """Decorator to memoize a method.
    Example
    -------
    class MyClass:
        @memoize
        def a_method(self):
            print("a_method called")
            return 42
    >>> my_object = MyClass()
    >>> my_object.a_method
    a_method called
    42
    >>> my_object.a_method
    42
    """
    attr_name = "_{}".format(fn.__name__)

    @wraps(fn)
    def memoized(self):
        """"memoized wraps"""
        if not hasattr(self, attr_name):
            setattr(self, attr_name, fn(self))
        return getattr(self, attr_name)

    return property(memoized)
</code>
</pre>
</details>

<h3><code>client.py</code> (or <a href="https://intranet-projects-files.s3.amazonaws.com/webstack/client.py" title="download" target="_blank">download</a>)</h3>

<details>
<summary>Click to show/hide file contents</summary>
<pre>
<code>
#!/usr/bin/env python3
"""A github org client
"""
from typing import (
    List,
    Dict,
)

from utils import (
    get_json,
    access_nested_map,
    memoize,
)


class GithubOrgClient:
    """A Githib org client
    """
    ORG_URL = "https://api.github.com/orgs/{org}"

    def __init__(self, org_name: str) -> None:
        """Init method of GithubOrgClient"""
        self._org_name = org_name

    @memoize
    def org(self) -> Dict:
        """Memoize org"""
        return get_json(self.ORG_URL.format(org=self._org_name))

    @property
    def _public_repos_url(self) -> str:
        """Public repos URL"""
        return self.org["repos_url"]

    @memoize
    def repos_payload(self) -> Dict:
        """Memoize repos payload"""
        return get_json(self._public_repos_url)

    def public_repos(self, license: str = None) -> List[str]:
        """Public repos"""
        json_payload = self.repos_payload
        public_repos = [
            repo["name"] for repo in json_payload
            if license is None or self.has_license(repo, license)
        ]

        return public_repos

    @staticmethod
    def has_license(repo: Dict[str, Dict], license_key: str) -> bool:
        """Static: has_license"""
        assert license_key is not None, "license_key cannot be None"
        try:
            has_license = access_nested_map(repo, ("license", "key")) == license_key
        except KeyError:
            return False
        return has_license
</code>
</pre>
</details>

<h3><code>fixtures.py</code> (or <a href="https://intranet-projects-files.s3.amazonaws.com/webstack/fixtures.py" title="download" target="_blank">download</a>)</h3>

<details>
<summary>Click to show/hide file contents</summary>
<pre>
<code>
#!/usr/bin/env python3

TEST_PAYLOAD = [
  (
    {"repos_url": "https://api.github.com/orgs/google/repos"},
    [
      {
        "id": 7697149,
        "node_id": "MDEwOlJlcG9zaXRvcnk3Njk3MTQ5",
        "name": "episodes.dart",
        "full_name": "google/episodes.dart",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/episodes.dart",
        "description": "A framework for timing performance of web apps.",
        "fork": False,
        "url": "https://api.github.com/repos/google/episodes.dart",
        "forks_url": "https://api.github.com/repos/google/episodes.dart/forks",
        "keys_url": "https://api.github.com/repos/google/episodes.dart/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/episodes.dart/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/episodes.dart/teams",
        "hooks_url": "https://api.github.com/repos/google/episodes.dart/hooks",
        "issue_events_url": "https://api.github.com/repos/google/episodes.dart/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/episodes.dart/events",
        "assignees_url": "https://api.github.com/repos/google/episodes.dart/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/episodes.dart/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/episodes.dart/tags",
        "blobs_url": "https://api.github.com/repos/google/episodes.dart/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/episodes.dart/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/episodes.dart/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/episodes.dart/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/episodes.dart/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/episodes.dart/languages",
        "stargazers_url": "https://api.github.com/repos/google/episodes.dart/stargazers",
        "contributors_url": "https://api.github.com/repos/google/episodes.dart/contributors",
        "subscribers_url": "https://api.github.com/repos/google/episodes.dart/subscribers",
        "subscription_url": "https://api.github.com/repos/google/episodes.dart/subscription",
        "commits_url": "https://api.github.com/repos/google/episodes.dart/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/episodes.dart/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/episodes.dart/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/episodes.dart/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/episodes.dart/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/episodes.dart/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/episodes.dart/merges",
        "archive_url": "https://api.github.com/repos/google/episodes.dart/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/episodes.dart/downloads",
        "issues_url": "https://api.github.com/repos/google/episodes.dart/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/episodes.dart/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/episodes.dart/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/episodes.dart/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/episodes.dart/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/episodes.dart/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/episodes.dart/deployments",
        "created_at": "2013-01-19T00:31:37Z",
        "updated_at": "2019-09-23T11:53:58Z",
        "pushed_at": "2014-10-09T21:39:33Z",
        "git_url": "git://github.com/google/episodes.dart.git",
        "ssh_url": "git@github.com:google/episodes.dart.git",
        "clone_url": "https://github.com/google/episodes.dart.git",
        "svn_url": "https://github.com/google/episodes.dart",
        "homepage": None,
        "size": 191,
        "stargazers_count": 12,
        "watchers_count": 12,
        "language": "Dart",
        "has_issues": True,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": True,
        "has_pages": False,
        "forks_count": 22,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 0,
        "license": {
          "key": "bsd-3-clause",
          "name": "BSD 3-Clause \"New\" or \"Revised\" License",
          "spdx_id": "BSD-3-Clause",
          "url": "https://api.github.com/licenses/bsd-3-clause",
          "node_id": "MDc6TGljZW5zZTU="
        },
        "forks": 22,
        "open_issues": 0,
        "watchers": 12,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 7776515,
        "node_id": "MDEwOlJlcG9zaXRvcnk3Nzc2NTE1",
        "name": "cpp-netlib",
        "full_name": "google/cpp-netlib",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/cpp-netlib",
        "description": "The C++ Network Library Project -- header-only, cross-platform, standards compliant networking library.",
        "fork": True,
        "url": "https://api.github.com/repos/google/cpp-netlib",
        "forks_url": "https://api.github.com/repos/google/cpp-netlib/forks",
        "keys_url": "https://api.github.com/repos/google/cpp-netlib/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/cpp-netlib/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/cpp-netlib/teams",
        "hooks_url": "https://api.github.com/repos/google/cpp-netlib/hooks",
        "issue_events_url": "https://api.github.com/repos/google/cpp-netlib/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/cpp-netlib/events",
        "assignees_url": "https://api.github.com/repos/google/cpp-netlib/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/cpp-netlib/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/cpp-netlib/tags",
        "blobs_url": "https://api.github.com/repos/google/cpp-netlib/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/cpp-netlib/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/cpp-netlib/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/cpp-netlib/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/cpp-netlib/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/cpp-netlib/languages",
        "stargazers_url": "https://api.github.com/repos/google/cpp-netlib/stargazers",
        "contributors_url": "https://api.github.com/repos/google/cpp-netlib/contributors",
        "subscribers_url": "https://api.github.com/repos/google/cpp-netlib/subscribers",
        "subscription_url": "https://api.github.com/repos/google/cpp-netlib/subscription",
        "commits_url": "https://api.github.com/repos/google/cpp-netlib/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/cpp-netlib/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/cpp-netlib/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/cpp-netlib/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/cpp-netlib/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/cpp-netlib/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/cpp-netlib/merges",
        "archive_url": "https://api.github.com/repos/google/cpp-netlib/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/cpp-netlib/downloads",
        "issues_url": "https://api.github.com/repos/google/cpp-netlib/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/cpp-netlib/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/cpp-netlib/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/cpp-netlib/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/cpp-netlib/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/cpp-netlib/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/cpp-netlib/deployments",
        "created_at": "2013-01-23T14:45:32Z",
        "updated_at": "2019-11-15T02:26:31Z",
        "pushed_at": "2018-12-05T17:42:29Z",
        "git_url": "git://github.com/google/cpp-netlib.git",
        "ssh_url": "git@github.com:google/cpp-netlib.git",
        "clone_url": "https://github.com/google/cpp-netlib.git",
        "svn_url": "https://github.com/google/cpp-netlib",
        "homepage": "http://cpp-netlib.github.com/",
        "size": 8937,
        "stargazers_count": 292,
        "watchers_count": 292,
        "language": "C++",
        "has_issues": False,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": True,
        "has_pages": False,
        "forks_count": 59,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 0,
        "license": {
          "key": "bsl-1.0",
          "name": "Boost Software License 1.0",
          "spdx_id": "BSL-1.0",
          "url": "https://api.github.com/licenses/bsl-1.0",
          "node_id": "MDc6TGljZW5zZTI4"
        },
        "forks": 59,
        "open_issues": 0,
        "watchers": 292,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 7968417,
        "node_id": "MDEwOlJlcG9zaXRvcnk3OTY4NDE3",
        "name": "dagger",
        "full_name": "google/dagger",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/dagger",
        "description": "A fast dependency injector for Android and Java.",
        "fork": True,
        "url": "https://api.github.com/repos/google/dagger",
        "forks_url": "https://api.github.com/repos/google/dagger/forks",
        "keys_url": "https://api.github.com/repos/google/dagger/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/dagger/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/dagger/teams",
        "hooks_url": "https://api.github.com/repos/google/dagger/hooks",
        "issue_events_url": "https://api.github.com/repos/google/dagger/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/dagger/events",
        "assignees_url": "https://api.github.com/repos/google/dagger/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/dagger/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/dagger/tags",
        "blobs_url": "https://api.github.com/repos/google/dagger/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/dagger/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/dagger/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/dagger/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/dagger/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/dagger/languages",
        "stargazers_url": "https://api.github.com/repos/google/dagger/stargazers",
        "contributors_url": "https://api.github.com/repos/google/dagger/contributors",
        "subscribers_url": "https://api.github.com/repos/google/dagger/subscribers",
        "subscription_url": "https://api.github.com/repos/google/dagger/subscription",
        "commits_url": "https://api.github.com/repos/google/dagger/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/dagger/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/dagger/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/dagger/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/dagger/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/dagger/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/dagger/merges",
        "archive_url": "https://api.github.com/repos/google/dagger/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/dagger/downloads",
        "issues_url": "https://api.github.com/repos/google/dagger/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/dagger/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/dagger/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/dagger/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/dagger/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/dagger/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/dagger/deployments",
        "created_at": "2013-02-01T23:14:14Z",
        "updated_at": "2019-12-03T12:39:55Z",
        "pushed_at": "2019-11-27T21:20:38Z",
        "git_url": "git://github.com/google/dagger.git",
        "ssh_url": "git@github.com:google/dagger.git",
        "clone_url": "https://github.com/google/dagger.git",
        "svn_url": "https://github.com/google/dagger",
        "homepage": "https://dagger.dev",
        "size": 59129,
        "stargazers_count": 14492,
        "watchers_count": 14492,
        "language": "Java",
        "has_issues": True,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": True,
        "has_pages": True,
        "forks_count": 1741,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 148,
        "license": {
          "key": "apache-2.0",
          "name": "Apache License 2.0",
          "spdx_id": "Apache-2.0",
          "url": "https://api.github.com/licenses/apache-2.0",
          "node_id": "MDc6TGljZW5zZTI="
        },
        "forks": 1741,
        "open_issues": 148,
        "watchers": 14492,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 8165161,
        "node_id": "MDEwOlJlcG9zaXRvcnk4MTY1MTYx",
        "name": "ios-webkit-debug-proxy",
        "full_name": "google/ios-webkit-debug-proxy",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/ios-webkit-debug-proxy",
        "description": "A DevTools proxy (Chrome Remote Debugging Protocol) for iOS devices (Safari Remote Web Inspector).",
        "fork": False,
        "url": "https://api.github.com/repos/google/ios-webkit-debug-proxy",
        "forks_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/forks",
        "keys_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/teams",
        "hooks_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/hooks",
        "issue_events_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/events",
        "assignees_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/tags",
        "blobs_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/languages",
        "stargazers_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/stargazers",
        "contributors_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/contributors",
        "subscribers_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/subscribers",
        "subscription_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/subscription",
        "commits_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/merges",
        "archive_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/downloads",
        "issues_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/ios-webkit-debug-proxy/deployments",
        "created_at": "2013-02-12T19:08:19Z",
        "updated_at": "2019-12-04T02:06:43Z",
        "pushed_at": "2019-11-24T07:02:13Z",
        "git_url": "git://github.com/google/ios-webkit-debug-proxy.git",
        "ssh_url": "git@github.com:google/ios-webkit-debug-proxy.git",
        "clone_url": "https://github.com/google/ios-webkit-debug-proxy.git",
        "svn_url": "https://github.com/google/ios-webkit-debug-proxy",
        "homepage": "",
        "size": 680,
        "stargazers_count": 4630,
        "watchers_count": 4630,
        "language": "C",
        "has_issues": True,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": False,
        "has_pages": False,
        "forks_count": 395,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 24,
        "license": {
          "key": "other",
          "name": "Other",
          "spdx_id": "NOASSERTION",
          "url": None,
          "node_id": "MDc6TGljZW5zZTA="
        },
        "forks": 395,
        "open_issues": 24,
        "watchers": 4630,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 8459994,
        "node_id": "MDEwOlJlcG9zaXRvcnk4NDU5OTk0",
        "name": "google.github.io",
        "full_name": "google/google.github.io",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/google.github.io",
        "description": None,
        "fork": False,
        "url": "https://api.github.com/repos/google/google.github.io",
        "forks_url": "https://api.github.com/repos/google/google.github.io/forks",
        "keys_url": "https://api.github.com/repos/google/google.github.io/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/google.github.io/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/google.github.io/teams",
        "hooks_url": "https://api.github.com/repos/google/google.github.io/hooks",
        "issue_events_url": "https://api.github.com/repos/google/google.github.io/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/google.github.io/events",
        "assignees_url": "https://api.github.com/repos/google/google.github.io/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/google.github.io/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/google.github.io/tags",
        "blobs_url": "https://api.github.com/repos/google/google.github.io/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/google.github.io/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/google.github.io/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/google.github.io/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/google.github.io/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/google.github.io/languages",
        "stargazers_url": "https://api.github.com/repos/google/google.github.io/stargazers",
        "contributors_url": "https://api.github.com/repos/google/google.github.io/contributors",
        "subscribers_url": "https://api.github.com/repos/google/google.github.io/subscribers",
        "subscription_url": "https://api.github.com/repos/google/google.github.io/subscription",
        "commits_url": "https://api.github.com/repos/google/google.github.io/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/google.github.io/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/google.github.io/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/google.github.io/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/google.github.io/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/google.github.io/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/google.github.io/merges",
        "archive_url": "https://api.github.com/repos/google/google.github.io/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/google.github.io/downloads",
        "issues_url": "https://api.github.com/repos/google/google.github.io/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/google.github.io/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/google.github.io/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/google.github.io/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/google.github.io/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/google.github.io/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/google.github.io/deployments",
        "created_at": "2013-02-27T16:21:19Z",
        "updated_at": "2019-12-03T01:38:02Z",
        "pushed_at": "2019-12-03T01:37:58Z",
        "git_url": "git://github.com/google/google.github.io.git",
        "ssh_url": "git@github.com:google/google.github.io.git",
        "clone_url": "https://github.com/google/google.github.io.git",
        "svn_url": "https://github.com/google/google.github.io",
        "homepage": None,
        "size": 8,
        "stargazers_count": 38,
        "watchers_count": 38,
        "language": "HTML",
        "has_issues": False,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": False,
        "has_pages": True,
        "forks_count": 44,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 0,
        "license": None,
        "forks": 44,
        "open_issues": 0,
        "watchers": 38,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 8566972,
        "node_id": "MDEwOlJlcG9zaXRvcnk4NTY2OTcy",
        "name": "kratu",
        "full_name": "google/kratu",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/kratu",
        "description": None,
        "fork": False,
        "url": "https://api.github.com/repos/google/kratu",
        "forks_url": "https://api.github.com/repos/google/kratu/forks",
        "keys_url": "https://api.github.com/repos/google/kratu/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/kratu/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/kratu/teams",
        "hooks_url": "https://api.github.com/repos/google/kratu/hooks",
        "issue_events_url": "https://api.github.com/repos/google/kratu/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/kratu/events",
        "assignees_url": "https://api.github.com/repos/google/kratu/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/kratu/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/kratu/tags",
        "blobs_url": "https://api.github.com/repos/google/kratu/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/kratu/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/kratu/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/kratu/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/kratu/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/kratu/languages",
        "stargazers_url": "https://api.github.com/repos/google/kratu/stargazers",
        "contributors_url": "https://api.github.com/repos/google/kratu/contributors",
        "subscribers_url": "https://api.github.com/repos/google/kratu/subscribers",
        "subscription_url": "https://api.github.com/repos/google/kratu/subscription",
        "commits_url": "https://api.github.com/repos/google/kratu/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/kratu/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/kratu/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/kratu/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/kratu/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/kratu/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/kratu/merges",
        "archive_url": "https://api.github.com/repos/google/kratu/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/kratu/downloads",
        "issues_url": "https://api.github.com/repos/google/kratu/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/kratu/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/kratu/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/kratu/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/kratu/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/kratu/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/kratu/deployments",
        "created_at": "2013-03-04T22:52:33Z",
        "updated_at": "2019-11-15T22:22:16Z",
        "pushed_at": "2017-08-06T05:44:34Z",
        "git_url": "git://github.com/google/kratu.git",
        "ssh_url": "git@github.com:google/kratu.git",
        "clone_url": "https://github.com/google/kratu.git",
        "svn_url": "https://github.com/google/kratu",
        "homepage": None,
        "size": 1777,
        "stargazers_count": 280,
        "watchers_count": 280,
        "language": "JavaScript",
        "has_issues": True,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": True,
        "has_pages": True,
        "forks_count": 32,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 0,
        "license": {
          "key": "apache-2.0",
          "name": "Apache License 2.0",
          "spdx_id": "Apache-2.0",
          "url": "https://api.github.com/licenses/apache-2.0",
          "node_id": "MDc6TGljZW5zZTI="
        },
        "forks": 32,
        "open_issues": 0,
        "watchers": 280,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 8858648,
        "node_id": "MDEwOlJlcG9zaXRvcnk4ODU4NjQ4",
        "name": "build-debian-cloud",
        "full_name": "google/build-debian-cloud",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/build-debian-cloud",
        "description": "Script to create Debian Squeeze & Wheezy Amazon Machine Images (AMIs) and Google Compute Engine images",
        "fork": True,
        "url": "https://api.github.com/repos/google/build-debian-cloud",
        "forks_url": "https://api.github.com/repos/google/build-debian-cloud/forks",
        "keys_url": "https://api.github.com/repos/google/build-debian-cloud/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/build-debian-cloud/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/build-debian-cloud/teams",
        "hooks_url": "https://api.github.com/repos/google/build-debian-cloud/hooks",
        "issue_events_url": "https://api.github.com/repos/google/build-debian-cloud/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/build-debian-cloud/events",
        "assignees_url": "https://api.github.com/repos/google/build-debian-cloud/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/build-debian-cloud/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/build-debian-cloud/tags",
        "blobs_url": "https://api.github.com/repos/google/build-debian-cloud/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/build-debian-cloud/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/build-debian-cloud/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/build-debian-cloud/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/build-debian-cloud/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/build-debian-cloud/languages",
        "stargazers_url": "https://api.github.com/repos/google/build-debian-cloud/stargazers",
        "contributors_url": "https://api.github.com/repos/google/build-debian-cloud/contributors",
        "subscribers_url": "https://api.github.com/repos/google/build-debian-cloud/subscribers",
        "subscription_url": "https://api.github.com/repos/google/build-debian-cloud/subscription",
        "commits_url": "https://api.github.com/repos/google/build-debian-cloud/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/build-debian-cloud/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/build-debian-cloud/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/build-debian-cloud/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/build-debian-cloud/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/build-debian-cloud/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/build-debian-cloud/merges",
        "archive_url": "https://api.github.com/repos/google/build-debian-cloud/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/build-debian-cloud/downloads",
        "issues_url": "https://api.github.com/repos/google/build-debian-cloud/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/build-debian-cloud/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/build-debian-cloud/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/build-debian-cloud/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/build-debian-cloud/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/build-debian-cloud/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/build-debian-cloud/deployments",
        "created_at": "2013-03-18T16:32:00Z",
        "updated_at": "2019-09-23T11:54:00Z",
        "pushed_at": "2014-06-17T18:52:10Z",
        "git_url": "git://github.com/google/build-debian-cloud.git",
        "ssh_url": "git@github.com:google/build-debian-cloud.git",
        "clone_url": "https://github.com/google/build-debian-cloud.git",
        "svn_url": "https://github.com/google/build-debian-cloud",
        "homepage": "",
        "size": 986,
        "stargazers_count": 32,
        "watchers_count": 32,
        "language": "Shell",
        "has_issues": False,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": False,
        "has_pages": False,
        "forks_count": 22,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 5,
        "license": {
          "key": "other",
          "name": "Other",
          "spdx_id": "NOASSERTION",
          "url": None,
          "node_id": "MDc6TGljZW5zZTA="
        },
        "forks": 22,
        "open_issues": 5,
        "watchers": 32,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 9060347,
        "node_id": "MDEwOlJlcG9zaXRvcnk5MDYwMzQ3",
        "name": "traceur-compiler",
        "full_name": "google/traceur-compiler",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/traceur-compiler",
        "description": "Traceur is a JavaScript.next-to-JavaScript-of-today compiler",
        "fork": False,
        "url": "https://api.github.com/repos/google/traceur-compiler",
        "forks_url": "https://api.github.com/repos/google/traceur-compiler/forks",
        "keys_url": "https://api.github.com/repos/google/traceur-compiler/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/traceur-compiler/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/traceur-compiler/teams",
        "hooks_url": "https://api.github.com/repos/google/traceur-compiler/hooks",
        "issue_events_url": "https://api.github.com/repos/google/traceur-compiler/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/traceur-compiler/events",
        "assignees_url": "https://api.github.com/repos/google/traceur-compiler/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/traceur-compiler/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/traceur-compiler/tags",
        "blobs_url": "https://api.github.com/repos/google/traceur-compiler/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/traceur-compiler/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/traceur-compiler/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/traceur-compiler/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/traceur-compiler/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/traceur-compiler/languages",
        "stargazers_url": "https://api.github.com/repos/google/traceur-compiler/stargazers",
        "contributors_url": "https://api.github.com/repos/google/traceur-compiler/contributors",
        "subscribers_url": "https://api.github.com/repos/google/traceur-compiler/subscribers",
        "subscription_url": "https://api.github.com/repos/google/traceur-compiler/subscription",
        "commits_url": "https://api.github.com/repos/google/traceur-compiler/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/traceur-compiler/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/traceur-compiler/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/traceur-compiler/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/traceur-compiler/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/traceur-compiler/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/traceur-compiler/merges",
        "archive_url": "https://api.github.com/repos/google/traceur-compiler/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/traceur-compiler/downloads",
        "issues_url": "https://api.github.com/repos/google/traceur-compiler/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/traceur-compiler/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/traceur-compiler/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/traceur-compiler/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/traceur-compiler/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/traceur-compiler/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/traceur-compiler/deployments",
        "created_at": "2013-03-27T18:05:40Z",
        "updated_at": "2019-12-02T16:45:54Z",
        "pushed_at": "2018-05-28T04:37:54Z",
        "git_url": "git://github.com/google/traceur-compiler.git",
        "ssh_url": "git@github.com:google/traceur-compiler.git",
        "clone_url": "https://github.com/google/traceur-compiler.git",
        "svn_url": "https://github.com/google/traceur-compiler",
        "homepage": "",
        "size": 27487,
        "stargazers_count": 8033,
        "watchers_count": 8033,
        "language": "JavaScript",
        "has_issues": True,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": True,
        "has_pages": True,
        "forks_count": 604,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 296,
        "license": {
          "key": "apache-2.0",
          "name": "Apache License 2.0",
          "spdx_id": "Apache-2.0",
          "url": "https://api.github.com/licenses/apache-2.0",
          "node_id": "MDc6TGljZW5zZTI="
        },
        "forks": 604,
        "open_issues": 296,
        "watchers": 8033,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      },
      {
        "id": 9065917,
        "node_id": "MDEwOlJlcG9zaXRvcnk5MDY1OTE3",
        "name": "firmata.py",
        "full_name": "google/firmata.py",
        "private": False,
        "owner": {
          "login": "google",
          "id": 1342004,
          "node_id": "MDEyOk9yZ2FuaXphdGlvbjEzNDIwMDQ=",
          "avatar_url": "https://avatars1.githubusercontent.com/u/1342004?v=4",
          "gravatar_id": "",
          "url": "https://api.github.com/users/google",
          "html_url": "https://github.com/google",
          "followers_url": "https://api.github.com/users/google/followers",
          "following_url": "https://api.github.com/users/google/following{/other_user}",
          "gists_url": "https://api.github.com/users/google/gists{/gist_id}",
          "starred_url": "https://api.github.com/users/google/starred{/owner}{/repo}",
          "subscriptions_url": "https://api.github.com/users/google/subscriptions",
          "organizations_url": "https://api.github.com/users/google/orgs",
          "repos_url": "https://api.github.com/users/google/repos",
          "events_url": "https://api.github.com/users/google/events{/privacy}",
          "received_events_url": "https://api.github.com/users/google/received_events",
          "type": "Organization",
          "site_admin": False
        },
        "html_url": "https://github.com/google/firmata.py",
        "description": None,
        "fork": False,
        "url": "https://api.github.com/repos/google/firmata.py",
        "forks_url": "https://api.github.com/repos/google/firmata.py/forks",
        "keys_url": "https://api.github.com/repos/google/firmata.py/keys{/key_id}",
        "collaborators_url": "https://api.github.com/repos/google/firmata.py/collaborators{/collaborator}",
        "teams_url": "https://api.github.com/repos/google/firmata.py/teams",
        "hooks_url": "https://api.github.com/repos/google/firmata.py/hooks",
        "issue_events_url": "https://api.github.com/repos/google/firmata.py/issues/events{/number}",
        "events_url": "https://api.github.com/repos/google/firmata.py/events",
        "assignees_url": "https://api.github.com/repos/google/firmata.py/assignees{/user}",
        "branches_url": "https://api.github.com/repos/google/firmata.py/branches{/branch}",
        "tags_url": "https://api.github.com/repos/google/firmata.py/tags",
        "blobs_url": "https://api.github.com/repos/google/firmata.py/git/blobs{/sha}",
        "git_tags_url": "https://api.github.com/repos/google/firmata.py/git/tags{/sha}",
        "git_refs_url": "https://api.github.com/repos/google/firmata.py/git/refs{/sha}",
        "trees_url": "https://api.github.com/repos/google/firmata.py/git/trees{/sha}",
        "statuses_url": "https://api.github.com/repos/google/firmata.py/statuses/{sha}",
        "languages_url": "https://api.github.com/repos/google/firmata.py/languages",
        "stargazers_url": "https://api.github.com/repos/google/firmata.py/stargazers",
        "contributors_url": "https://api.github.com/repos/google/firmata.py/contributors",
        "subscribers_url": "https://api.github.com/repos/google/firmata.py/subscribers",
        "subscription_url": "https://api.github.com/repos/google/firmata.py/subscription",
        "commits_url": "https://api.github.com/repos/google/firmata.py/commits{/sha}",
        "git_commits_url": "https://api.github.com/repos/google/firmata.py/git/commits{/sha}",
        "comments_url": "https://api.github.com/repos/google/firmata.py/comments{/number}",
        "issue_comment_url": "https://api.github.com/repos/google/firmata.py/issues/comments{/number}",
        "contents_url": "https://api.github.com/repos/google/firmata.py/contents/{+path}",
        "compare_url": "https://api.github.com/repos/google/firmata.py/compare/{base}...{head}",
        "merges_url": "https://api.github.com/repos/google/firmata.py/merges",
        "archive_url": "https://api.github.com/repos/google/firmata.py/{archive_format}{/ref}",
        "downloads_url": "https://api.github.com/repos/google/firmata.py/downloads",
        "issues_url": "https://api.github.com/repos/google/firmata.py/issues{/number}",
        "pulls_url": "https://api.github.com/repos/google/firmata.py/pulls{/number}",
        "milestones_url": "https://api.github.com/repos/google/firmata.py/milestones{/number}",
        "notifications_url": "https://api.github.com/repos/google/firmata.py/notifications{?since,all,participating}",
        "labels_url": "https://api.github.com/repos/google/firmata.py/labels{/name}",
        "releases_url": "https://api.github.com/repos/google/firmata.py/releases{/id}",
        "deployments_url": "https://api.github.com/repos/google/firmata.py/deployments",
        "created_at": "2013-03-27T23:20:35Z",
        "updated_at": "2019-09-23T11:54:02Z",
        "pushed_at": "2013-03-27T23:34:35Z",
        "git_url": "git://github.com/google/firmata.py.git",
        "ssh_url": "git@github.com:google/firmata.py.git",
        "clone_url": "https://github.com/google/firmata.py.git",
        "svn_url": "https://github.com/google/firmata.py",
        "homepage": None,
        "size": 160,
        "stargazers_count": 15,
        "watchers_count": 15,
        "language": "Python",
        "has_issues": True,
        "has_projects": True,
        "has_downloads": True,
        "has_wiki": True,
        "has_pages": False,
        "forks_count": 15,
        "mirror_url": None,
        "archived": False,
        "disabled": False,
        "open_issues_count": 0,
        "license": {
          "key": "apache-2.0",
          "name": "Apache License 2.0",
          "spdx_id": "Apache-2.0",
          "url": "https://api.github.com/licenses/apache-2.0",
          "node_id": "MDc6TGljZW5zZTI="
        },
        "forks": 15,
        "open_issues": 0,
        "watchers": 15,
        "default_branch": "master",
        "permissions": {
          "admin": False,
          "push": False,
          "pull": True
        }
      }
    ],
    ['episodes.dart', 'cpp-netlib', 'dagger', 'ios-webkit-debug-proxy', 'google.github.io', 'kratu', 'build-debian-cloud', 'traceur-compiler', 'firmata.py'],
    ['dagger', 'kratu', 'traceur-compiler', 'firmata.py'],
  )
]
</code>
</pre>
</details>

  </div>
</div>


      

      

        
          <h2 class="gap">Tasks</h2>

    <div data-role="task11679" data-position="1" id="task-num-0">
      <div class="panel panel-default task-card " id="task-11679">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      0. Parameterize a unit test
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11679" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Familiarize yourself with the <code>utils.access_nested_map</code> function and understand its purpose. Play with it in the Python console to make sure you understand.</p>

<p>In this task you will write the first unit test for <code>utils.access_nested_map</code>.</p>

<p>Create a <code>TestAccessNestedMap</code> class that inherits from <code>unittest.TestCase</code>.</p>

<p>Implement the <code>TestAccessNestedMap.test_access_nested_map</code> method to test that the method returns what it is supposed to.</p>

<p>Decorate the method with <code>@parameterized.expand</code> to test the function for following inputs:</p>

<pre><code>nested_map={&quot;a&quot;: 1}, path=(&quot;a&quot;,)
nested_map={&quot;a&quot;: {&quot;b&quot;: 2}}, path=(&quot;a&quot;,)
nested_map={&quot;a&quot;: {&quot;b&quot;: 2}}, path=(&quot;a&quot;, &quot;b&quot;)
</code></pre>

<p>For each of these inputs, test with <code>assertEqual</code> that the function returns the expected result.</p>

<p>The body of the test method should not be longer than 2 lines.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_utils.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11679">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11679" data-batch-id="58" data-toggle="modal" data-target="#task-11679-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11679-users-done-modal" data-task-id="11679" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "0. Parameterize a unit test"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11679-modal-button" data-task-id="11679" data-toggle="modal" data-target="#task-test-correction-11679-correction-modal" id="task-num-0-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11679}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11679-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "0. Parameterize a unit test"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11679">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11679">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11679">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11679" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11679}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11679" data-toggle="modal" data-target="#task-qa-review-11679-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11679}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11679-modal" data-correction-id="20835096" data-task-id="11679">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">0. Parameterize a unit test</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11680" data-position="2" id="task-num-1">
      <div class="panel panel-default task-card " id="task-11680">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      1. Parameterize a unit test
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11680" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Implement <code>TestAccessNestedMap.test_access_nested_map_exception</code>. Use the <code>assertRaises</code> context manager to test that a <code>KeyError</code> is raised for the following inputs (use <code>@parameterized.expand</code>):</p>

<pre><code>nested_map={}, path=(&quot;a&quot;,)
nested_map={&quot;a&quot;: 1}, path=(&quot;a&quot;, &quot;b&quot;)
</code></pre>

<p>Also make sure that the exception message is as expected.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_utils.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11680">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11680" data-batch-id="58" data-toggle="modal" data-target="#task-11680-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11680-users-done-modal" data-task-id="11680" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "1. Parameterize a unit test"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11680-modal-button" data-task-id="11680" data-toggle="modal" data-target="#task-test-correction-11680-correction-modal" id="task-num-1-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11680}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11680-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "1. Parameterize a unit test"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11680">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11680">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11680">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11680" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11680}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11680" data-toggle="modal" data-target="#task-qa-review-11680-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11680}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11680-modal" data-correction-id="20835096" data-task-id="11680">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">1. Parameterize a unit test</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11681" data-position="3" id="task-num-2">
      <div class="panel panel-default task-card " id="task-11681">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      2. Mock HTTP calls
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11681" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Familiarize yourself with the <code>utils.get_json</code> function.</p>

<p>Define the <code>TestGetJson(unittest.TestCase)</code> class and implement the <code>TestGetJson.test_get_json</code> method to test that <code>utils.get_json</code> returns the expected result.</p>

<p>We don&rsquo;t want to make any actual external HTTP calls. Use <code>unittest.mock.patch</code> to patch <code>requests.get</code>. Make sure it returns a <code>Mock</code> object with a <code>json</code> method that returns <code>test_payload</code> which you parametrize alongside the <code>test_url</code> that you will pass to <code>get_json</code> with the following inputs:</p>

<pre><code>test_url=&quot;http://example.com&quot;, test_payload={&quot;payload&quot;: True}
test_url=&quot;http://holberton.io&quot;, test_payload={&quot;payload&quot;: False}
</code></pre>

<p>Test that the mocked <code>get</code> method was called exactly once (per input) with <code>test_url</code> as argument.</p>

<p>Test that the output of <code>get_json</code> is equal to <code>test_payload</code>.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_utils.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11681">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11681" data-batch-id="58" data-toggle="modal" data-target="#task-11681-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11681-users-done-modal" data-task-id="11681" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "2. Mock HTTP calls"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11681-modal-button" data-task-id="11681" data-toggle="modal" data-target="#task-test-correction-11681-correction-modal" id="task-num-2-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11681}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11681-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "2. Mock HTTP calls"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11681">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11681">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11681">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11681" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11681}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11681" data-toggle="modal" data-target="#task-qa-review-11681-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11681}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11681-modal" data-correction-id="20835096" data-task-id="11681">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">2. Mock HTTP calls</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11682" data-position="4" id="task-num-3">
      <div class="panel panel-default task-card " id="task-11682">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      3. Parameterize and patch
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11682" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Read about memoization and familiarize yourself with the <code>utils.memoize</code> decorator.</p>

<p>Implement the <code>TestMemoize(unittest.TestCase)</code> class with a <code>test_memoize</code> method.</p>

<p>Inside <code>test_memoize</code>, define following class</p>

<pre><code class="python">class TestClass:

    def a_method(self):
        return 42

    @memoize
    def a_property(self):
        return self.a_method()
</code></pre>

<p>Use <code>unittest.mock.patch</code> to mock <code>a_method</code>. Test that when calling <code>a_property</code> twice, the correct result is returned but <code>a_method</code> is only called once using <code>assert_called_once</code>.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_utils.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11682">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11682" data-batch-id="58" data-toggle="modal" data-target="#task-11682-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11682-users-done-modal" data-task-id="11682" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "3. Parameterize and patch"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11682-modal-button" data-task-id="11682" data-toggle="modal" data-target="#task-test-correction-11682-correction-modal" id="task-num-3-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11682}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11682-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "3. Parameterize and patch"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11682">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11682">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11682">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11682" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11682}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11682" data-toggle="modal" data-target="#task-qa-review-11682-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11682}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11682-modal" data-correction-id="20835096" data-task-id="11682">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">3. Parameterize and patch</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11683" data-position="5" id="task-num-4">
      <div class="panel panel-default task-card " id="task-11683">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      4. Parameterize and patch as decorators
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11683" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Familiarize yourself with the <code>client.GithubOrgClient</code> class.</p>

<p>In a new <code>test_client.py</code> file, declare the <code>TestGithubOrgClient(unittest.TestCase)</code> class and implement the <code>test_org</code> method.</p>

<p>This method should test that <code>GithubOrgClient.org</code> returns the correct value.</p>

<p>Use <code>@patch</code> as a decorator to make sure <code>get_json</code> is called once with the expected argument but make sure it is not executed.</p>

<p>Use <code>@parameterized.expand</code> as a decorator to parametrize the test with a couple of <code>org</code> examples to pass to <code>GithubOrgClient</code>, in this order:</p>

<ul>
<li><code>google</code></li>
<li><code>abc</code></li>
</ul>

<p>Of course, no external HTTP calls should be made.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_client.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11683">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11683" data-batch-id="58" data-toggle="modal" data-target="#task-11683-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11683-users-done-modal" data-task-id="11683" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "4. Parameterize and patch as decorators"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11683-modal-button" data-task-id="11683" data-toggle="modal" data-target="#task-test-correction-11683-correction-modal" id="task-num-4-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11683}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11683-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "4. Parameterize and patch as decorators"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11683">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11683">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11683">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11683" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11683}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11683" data-toggle="modal" data-target="#task-qa-review-11683-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11683}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11683-modal" data-correction-id="20835096" data-task-id="11683">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">4. Parameterize and patch as decorators</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11684" data-position="6" id="task-num-5">
      <div class="panel panel-default task-card " id="task-11684">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      5.  Mocking a property
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11684" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p><code>memoize</code> turns methods into properties. Read up on how to mock a property (see resource).</p>

<p>Implement the <code>test_public_repos_url</code> method to unit-test <code>GithubOrgClient._public_repos_url</code>.</p>

<p>Use <code>patch</code> as a context manager to patch <code>GithubOrgClient.org</code> and make it return a known payload.</p>

<p>Test that the result of <code>_public_repos_url</code> is the expected one based on the mocked payload.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_client.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11684">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11684" data-batch-id="58" data-toggle="modal" data-target="#task-11684-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11684-users-done-modal" data-task-id="11684" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "5.  Mocking a property"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11684-modal-button" data-task-id="11684" data-toggle="modal" data-target="#task-test-correction-11684-correction-modal" id="task-num-5-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11684}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11684-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "5.  Mocking a property"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11684">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11684">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11684">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11684" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11684}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11684" data-toggle="modal" data-target="#task-qa-review-11684-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11684}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11684-modal" data-correction-id="20835096" data-task-id="11684">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">5.  Mocking a property</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11685" data-position="7" id="task-num-6">
      <div class="panel panel-default task-card " id="task-11685">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      6. More patching
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11685" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Implement <code>TestGithubOrgClient.test_public_repos</code> to unit-test <code>GithubOrgClient.public_repos</code>.</p>

<p>Use <code>@patch</code> as a decorator to mock <code>get_json</code> and make it return a payload of your choice.</p>

<p>Use <code>patch</code> as a context manager to mock <code>GithubOrgClient._public_repos_url</code> and return a value of your choice.</p>

<p>Test that the list of repos is what you expect from the chosen payload.</p>

<p>Test that the mocked property and the mocked <code>get_json</code> was called once.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_client.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11685">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11685" data-batch-id="58" data-toggle="modal" data-target="#task-11685-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11685-users-done-modal" data-task-id="11685" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "6. More patching"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11685-modal-button" data-task-id="11685" data-toggle="modal" data-target="#task-test-correction-11685-correction-modal" id="task-num-6-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11685}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11685-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "6. More patching"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11685">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11685">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11685">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11685" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11685}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11685" data-toggle="modal" data-target="#task-qa-review-11685-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11685}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11685-modal" data-correction-id="20835096" data-task-id="11685">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">6. More patching</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11688" data-position="8" id="task-num-7">
      <div class="panel panel-default task-card " id="task-11688">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      7. Parameterize
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11688" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Implement <code>TestGithubOrgClient.test_has_license</code> to unit-test <code>GithubOrgClient.has_license</code>.</p>

<p>Parametrize the test with the following inputs</p>

<pre><code>repo={&quot;license&quot;: {&quot;key&quot;: &quot;my_license&quot;}}, license_key=&quot;my_license&quot;
repo={&quot;license&quot;: {&quot;key&quot;: &quot;other_license&quot;}}, license_key=&quot;my_license&quot;
</code></pre>

<p>You should also parameterize the expected returned value.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_client.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11688">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11688" data-batch-id="58" data-toggle="modal" data-target="#task-11688-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11688-users-done-modal" data-task-id="11688" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "7. Parameterize"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11688-modal-button" data-task-id="11688" data-toggle="modal" data-target="#task-test-correction-11688-correction-modal" id="task-num-7-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11688}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11688-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "7. Parameterize"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11688">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11688">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11688">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11688" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11688}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11688" data-toggle="modal" data-target="#task-qa-review-11688-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11688}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11688-modal" data-correction-id="20835096" data-task-id="11688">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">7. Parameterize</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11686" data-position="9" id="task-num-8">
      <div class="panel panel-default task-card " id="task-11686">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      8. Integration test: fixtures
    </h3>

    <div>
        <span class="label label-info">
          mandatory
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11686" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>We want to test the <code>GithubOrgClient.public_repos</code> method in an integration test. That means that we will only mock code that sends external requests.</p>

<p>Create the <code>TestIntegrationGithubOrgClient(unittest.TestCase)</code> class and implement the <code>setUpClass</code> and <code>tearDownClass</code> which are part of the <code>unittest.TestCase</code> API.</p>

<p>Use <code>@parameterized_class</code> to decorate the class and parameterize it with fixtures found in <code>fixtures.py</code>. The file contains the following fixtures:</p>

<pre><code>org_payload, repos_payload, expected_repos, apache2_repos
</code></pre>

<p>The <code>setupClass</code> should mock <code>requests.get</code> to return example payloads found in the fixtures.</p>

<p>Use <code>patch</code> to start a patcher named <code>get_patcher</code>, and use <code>side_effect</code> to make sure the mock of <code>requests.get(url).json()</code> returns the correct fixtures for the various values of <code>url</code> that you anticipate to receive.</p>

<p>Implement the <code>tearDownClass</code> class method to stop the patcher.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_client.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11686">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11686" data-batch-id="58" data-toggle="modal" data-target="#task-11686-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11686-users-done-modal" data-task-id="11686" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "8. Integration test: fixtures"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11686-modal-button" data-task-id="11686" data-toggle="modal" data-target="#task-test-correction-11686-correction-modal" id="task-num-8-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11686}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11686-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "8. Integration test: fixtures"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11686">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11686">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11686">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11686" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11686}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11686" data-toggle="modal" data-target="#task-qa-review-11686-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11686}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11686-modal" data-correction-id="20835096" data-task-id="11686">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">8. Integration test: fixtures</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>
    <div data-role="task11687" data-position="10" id="task-num-9">
      <div class="panel panel-default task-card " id="task-11687">
  <span id="user_id" data-id="220204"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      9. Integration tests
    </h3>

    <div>
        <span class="label label-info">
          #advanced
        </span>
    </div>
  </div>

  <div class="panel-body">
    <span id="user_id" data-id="220204"></span>

    <!-- Progress vs Score -->
      <div class="task_progress_score_bar" data-task-id="11687" data-correction-id="20835096">
        <div class="task_progress_bar" style="width: 0.0%">
          <div class="task_score_bar" style="width: NaN%">
          </div>
        </div>
        <div class="task_progress_score_text">
          Score: <span class="task_score_value">0.0%</span> (<span class="task_progress_value">Checks completed: 0.0%</span>)
        </div>
      </div>

    <!-- Task Body -->
    <p>Implement the <code>test_public_repos</code> method to test <code>GithubOrgClient.public_repos</code>.</p>

<p>Make sure that the method returns the expected results based on the fixtures.</p>

<p>Implement <code>test_public_repos_with_license</code>  to test the <code>public_repos</code> with the argument <code>license=&quot;apache-2.0&quot;</code> and make sure the result matches the expected value from the fixtures.</p>

  </div>

  <div class="list-group">
    <!-- Task URLs -->

    <!-- Github information -->
      <div class="list-group-item">
        <p><strong>Repo:</strong></p>
        <ul>
          <li>GitHub repository: <code>alx-backend-python</code></li>
            <li>Directory: <code>0x03-Unittests_and_integration_tests</code></li>
            <li>File: <code>test_client.py</code></li>
        </ul>
      </div>

    <!-- Self-paced manual review -->
  </div>

  <!-- Panel footer - Controls -->
  <div class="panel-footer">
      <div class="align-items-center d-flex justify-content-between">
        
<div>
    <button class="student_task_done btn btn-default btn-sm no" data-task-id="11687">
      <span class="no"><i aria-hidden="true" class="fa-regular fa-square "></i></span>
      <span class="yes"><i aria-hidden="true" class="fa-regular fa-square-check "></i></span>
      <span class="pending"><i aria-hidden="true" class="fa-solid fa-spinner  fa-spin-pulse"></i></span>
      Done<span class="no pending">?</span><span class="yes">!</span>
    </button>

  <button class="student-task-done-by btn btn-default btn-sm" data-task-id="11687" data-batch-id="58" data-toggle="modal" data-target="#task-11687-users-done-modal">
    Help
  </button>
  <div class="modal fade users-done-modal" id="task-11687-users-done-modal" data-task-id="11687" data-batch-id="58">
    <div class="modal-dialog">
        <div class="modal-content">
        <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title">Learners who are done with "9. Integration tests"</h4>
        </div>
        <div class="modal-body">
            <div class="list-group">
            </div>
            <div class="spinner">
                <div class="bounce1"></div>
                <div class="bounce2"></div>
                <div class="bounce3"></div>
            </div>
            <div class="error"></div>
        </div>
        </div>
    </div>
</div>


      <button class="btn btn-default btn-sm check-your-task-11687-modal-button" data-task-id="11687" data-toggle="modal" data-target="#task-test-correction-11687-correction-modal" id="task-num-9-check-code-btn" data-gtm-custom-event-name="task_checker_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11687}'>
          Check your code
      </button>
      <div class="modal fade task_correction_modal student_modal" id="task-test-correction-11687-correction-modal">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">Correction of "9. Integration tests"</h4>
            </div>
            <div class="modal-body">
                <div class="actions">
                    <center>
                        <div class="alert alert-info hidden"></div>

                        <button name="button" type="submit" class="btn btn-primary correction_request_test_send" data-task-id="11687">Start a new test</button>
                        <button class="btn btn-default close-modal hidden" data-dismiss="modal" type="button">Close</button>

                        <div class="spinner" style="display: none;">
                            <div class="bounce1"></div>
                            <div class="bounce2"></div>
                            <div class="bounce3"></div>
                        </div>
                        <div class="error"></div>
                        <div class="info"></div>
                    </center>
                </div>
                <div class="result"></div>

                <div class="help">
    <button data-task-id="11687">
        <i aria-hidden="true" class="fa-solid fa-circle-info "></i>
    </button>
    <div class="help-container" data-task-id="11687">
        <div class="check-line">
            <div class="check-inline requirement success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Requirement success
            </div>
            <div class="check-inline requirement fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Requirement fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline code success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Code success
            </div>
            <div class="check-inline code fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Code fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline efficiency success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Efficiency success
            </div>
            <div class="check-inline efficiency fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Efficiency fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline answer success">
                <i aria-hidden="true" class="fa-solid fa-circle-check "></i>
                Text answer success
            </div>
            <div class="check-inline answer fail">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Text answer fail
            </div>
        </div>
        <div class="check-line">
            <div class="check-inline requirement fail offline">
                <i aria-hidden="true" class="fa-solid fa-circle-xmark "></i>
                Skipped - Previous check failed
            </div>
        </div>
    </div>
</div>

            </div>
        </div>
    </div>
</div>


      <button class="btn btn-primary btn-sm task_ask_new_correction " data-task-id="11687" data-correction-id="20835096">
        Ask for a new correction
        <span class="in_progress_info">: in progress...</span>
        <span class="error_occurred_info">: an error occurred</span>
      </button>

    <button class="btn btn-default btn-sm" data-toggle="modal" data-target="#container-specs-modal" data-gtm-custom-event-name="task_sandbox_modal" data-gtm-custom-event-options="{&quot;taskId&quot;:11687}"><i aria-hidden="true" class="fa-solid fa-terminal "></i><span>Get a sandbox</span></button>

      <button class="btn btn-default btn-sm" data-task-id="11687" data-toggle="modal" data-target="#task-qa-review-11687-modal" data-gtm-custom-event-name="task_qa_review_modal" data-gtm-custom-event-options='{&quot;taskId&quot;:11687}'>
        QA Review
      </button>
      <div class="modal fade task_get_qa_review" id="task-qa-review-11687-modal" data-correction-id="20835096" data-task-id="11687">
    <div class="modal-dialog modal-lg">
        <div class="modal-content">
            <div class="modal-header">
                <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                <h4 class="modal-title">9. Integration tests</h4>
            </div>
            <div class="modal-body">
                <div class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div class="review-container">
                    <div class="review-corrector"></div>
                    <div class="review-github well" style="display:none">
                        <h5>Commit used:</h5>
                        <ul>
                            <li style="display:none"><strong>User:</strong> <code class="review-github-id"></code> <span class="review-github-name">---</span></li>
                            <li style="display:none"><strong>URL:</strong> <a class="review-github-url" target="_blank">Click here</a></li>
                            <li style="display:none"><strong>ID:</strong> <code class="review-github-commit_id">---</code></li>
                            <li style="display:none"><strong>Author:</strong> <span class="review-github-committer_username">---</span></li>
                            <li style="display:none"><strong>Subject:</strong> <em class="review-github-subject">---</em></li>
                            <li style="display:none"><strong>Date:</strong> <span class="review-github-datetime">---</span></li>
                        </ul>
                    </div>
                    <div class="review-percentage_down"></div>
                    <ul class="review-checks list-group sm-gap"></ul>
                    <div class="review-comment"></div>
                </div>
            </div>
        </div>
    </div>
</div>

</div>


        <div class="fs-4">
        </div>
      </div>


  </div>
</div>

    </div>





          <div class="modal fade" id="container-specs-modal"><div class="modal-dialog modal-lg"><div class="modal-content"><div class="modal-header"><button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button><h4 class="modal-title">Recommended Sandbox</h4></div><div class="modal-body"><div data-react-class="user_containers/ContainerSpecs" data-react-props="{&quot;containerModelName&quot;:&quot;Sandbox&quot;,&quot;containerSpecs&quot;:[{&quot;available&quot;:true,&quot;description&quot;:&quot;\u003cp\u003eUbuntu 18.04 with Python 3.7\u003c/p\u003e\n&quot;,&quot;id&quot;:23,&quot;name&quot;:&quot;Ubuntu 18.04 - Python 3.7&quot;,&quot;online&quot;:true,&quot;container&quot;:{&quot;container_id&quot;:&quot;1acd6693d9e1bb70846a05261c1bf512e4062670e7fdc437e4de1cc0daa993bd&quot;,&quot;id&quot;:590058,&quot;restart_uri&quot;:&quot;/user_containers/590058/restart.json&quot;,&quot;status&quot;:&quot;running&quot;,&quot;uri&quot;:&quot;/user_containers/590058.json&quot;,&quot;wake_uri&quot;:&quot;/user_containers/590058/wake.json&quot;,&quot;webterm_uri&quot;:&quot;/user_containers/590058/webterm&quot;,&quot;host&quot;:&quot;1acd6693d9e1.3e24de83.alx-cod.online&quot;,&quot;password&quot;:&quot;1a1ca237007682bed680&quot;,&quot;ports&quot;:{&quot;8080&quot;:53680,&quot;22&quot;:53687,&quot;3000&quot;:53685,&quot;4000&quot;:53684,&quot;5000&quot;:53683,&quot;5001&quot;:53682,&quot;80&quot;:53686,&quot;8000&quot;:53681}}}],&quot;containersLimit&quot;:2,&quot;csrfToken&quot;:&quot;CV1Qk24wiYTAgMXYcKo7vqeZin1QcQqqqPS0lKriB0T45ZIiQNgFEIMi8HPkDSQwqYBk3obVSkmHNLF1ZnMEDA&quot;,&quot;startStatusURI&quot;:&quot;/user_containers/start_status.json&quot;,&quot;startURI&quot;:&quot;/user_containers/start.json&quot;}" data-react-cache-id="user_containers/ContainerSpecs-0"></div></div></div></div></div>

  </div>
</div>


      </article>

      <div class="copyright">Copyright © 2023 ALX, All rights reserved.</div>

    </main>

        <button class="btn btn-primary" id="search-button" data-search-active="false" data-toggle="modal" data-target="#search-modal">
  <i aria-hidden="true" class="fa-solid fa-magnifying-glass "></i>
  <i aria-hidden="true" class="fa-solid fa-window-minimize "></i>
</button>

        <div class="modal fade" id="search-modal" tabindex="-1" role="dialog" aria-labelledby="search-modal-label">
    <div class="modal-dialog modal-md">
        <div class="modal-content">
            <div class="modal-header">
                <div id="search-bar-container">
    <input id="search-bar"
            autocomplete="off"
            type="text"
            name="hbtn-search-bar"
            placeholder="✨Start search by typing in this field✨">
</div>

            </div>
            <div class="modal-body">
                <div id="modal-spinner" class="spinner gap">
                    <div class="bounce1"></div>
                    <div class="bounce2"></div>
                    <div class="bounce3"></div>
                </div>
                <div id="search-results-container">
</div>

            </div>
        </div>
    </div>
</div>



        <div class="modal fade" id="markdownGuideModal" tabindex="-1" role="dialog" aria-labelledby="markdownGuideModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-md">
    <div class="modal-content">
        <div class="modal-header">
          <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
          <h4 class="modal-title">Markdown Guide</h4>
        </div>
        <div class="modal-body">
            <h4>Emphasis</h4>
<pre>**<strong>bold</strong>**
*<em>italics</em>*
~~<strike>strikethrough</strike>~~</pre>
<h4>Headers</h4>
<pre># Big header
## Medium header
### Small header
#### Tiny header</pre>
<h4>Lists</h4>
<pre>* Generic list item
* Generic list item
* Generic list item

1. Numbered list item
2. Numbered list item
3. Numbered list item</pre>
<h4>Links</h4>
<pre>[Text to display](http://www.example.com)</pre>
<h4>Quotes</h4>
<pre>> This is a quote.
> It can span multiple lines!</pre>
<h4>Images</h4>
<p>CSS style available: <code>width, height, opacity</code></p>
<pre>![](http://www.example.com/image.jpg)
![](http://www.example.com/image.jpg | width: 200px)
![](http://www.example.com/image.jpg | height: 124px | width: 80px | opacity: 0.6)
</pre>
<h4>Tables</h4>
<pre>| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| John     | Doe      | Male     |
| Mary     | Smith    | Female   |

<em>Or without aligning the columns...</em>

| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| John | Doe | Male |
| Mary | Smith | Female |
</pre>
<h4>Displaying code</h4>
<pre>`var example = "hello!";`

<em>Or spanning multiple lines...</em>

```
var example = "hello!";
alert(example);
```</pre>
        </div>
    </div>
  </div>
</div>


  </body>
</html>

