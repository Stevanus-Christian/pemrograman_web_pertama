
<!DOCTYPE html>


















































<html class="hasSidebar hasPageActions hasBreadcrumb conceptual has-default-focus theme-light" lang="en-us" dir="ltr" data-css-variable-support="true" data-authenticated="false" data-auth-status-determined="false" data-target="docs" x-ms-format-detection="none">

<head>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta property="og:title" content="Create a .NET console application using Visual Studio Code - .NET" />
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code" />
			<meta property="og:description" content="Learn how to create a .NET console application using Visual Studio Code and the .NET CLI." />
		<meta property="og:image" content="https://docs.microsoft.com/dotnet/media/dotnet-logo.svg" />
		<meta property="og:image:alt" content="Create a .NET console application using Visual Studio Code - .NET | Microsoft Docs" />

	<meta name="twitter:card" content="summary" />
	<meta name="twitter:site" content="@docsmsft" />

	<meta name="color-scheme" content="light dark">


	<meta name="apiPlatform" content="dotnet" />
<meta name="author" content="tdykstra" />
<meta name="breadcrumb_path" content="/dotnet/breadcrumb/toc.json" />
<meta name="depot_name" content="VS.core-docs" />
<meta name="description" content="Learn how to create a .NET console application using Visual Studio Code and the .NET CLI." />
<meta name="document_id" content="8cc2e9c2-f333-f6a1-064e-790d950b684c" />
<meta name="document_version_independent_id" content="25a4c9b9-2808-e296-df03-5837000dcbad" />
<meta name="gitcommit" content="https://github.com/dotnet/docs/blob/e56361206fc94a2a4fe4ea0b5e25acddf0b1667e/docs/core/tutorials/with-visual-studio-code.md" />
<meta name="locale" content="en-us" />
<meta name="ms.author" content="tdykstra" />
<meta name="ms.date" content="11/17/2020" />
<meta name="ms.devlang" content="dotnet" />
<meta name="ms.prod" content="dotnet-fundamentals" />
<meta name="ms.topic" content="tutorial" />
<meta name="original_content_git_url" content="https://github.com/dotnet/docs/blob/live/docs/core/tutorials/with-visual-studio-code.md" />
<meta name="recommendations" content="false" />
<meta name="schema" content="Conceptual" />
<meta name="search.ms_docsetname" content="core-docs" />
<meta name="search.ms_product" content="VS" />
<meta name="search.ms_sitename" content="Docs" />
<meta name="show_latex" content="true" />
<meta name="site_name" content="Docs" />
<meta name="uhfHeaderId" content="MSDocsHeader-DotNet" />
<meta name="updated_at" content="2021-05-21 10:29 AM" />
<meta name="page_type" content="conceptual" />
<meta name="toc_rel" content="../../fundamentals/toc.json" />
<meta name="pdf_url_template" content="https://docs.microsoft.com/pdfstore/en-us/VS.core-docs/{branchName}{pdfName}" />
<meta name="search.mshattr.devlang" content="csharp" />
<meta name="word_count" content="656" />


	<meta name="scope" content=".NET" />
<link href="https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code" rel="canonical">
	<title>Create a .NET console application using Visual Studio Code - .NET | Microsoft Docs</title>

		<link rel="stylesheet" href="/_themes/docs.theme/master/en-us/_themes/styles/b16628cd.site-ltr.css ">

	


	<script id="msdocs-script">
	var msDocs = {
		data: {
			timeOrigin: Date.now(),
			contentLocale: 'en-us',
			contentDir: 'ltr',
			userLocale: 'en-us',
			userDir: 'ltr',
			pageTemplate: 'Conceptual',
			brand: '',
			context: {

			},
			hasBinaryRating: true,
			hasGithubIssues: true,
			showFeedbackReport: false,
			enableTutorialFeedback: false,
			feedbackSystem: 'GitHub',
			feedbackGitHubRepo: 'dotnet/docs',
			feedbackProductUrl: 'https://aka.ms/feedback/report?space=61',
			contentGitUrl: 'https://github.com/dotnet/docs/blob/main/docs/core/tutorials/with-visual-studio-code.md',
			extendBreadcrumb: false,
			isEditDisplayable: true,
			hideViewSource: false,
			hasPageActions: true,
			hasBookmark: true,
			hasShare: true,
			hasRecommendations: true,
			contributors: [
						{ name: "tdykstra", url: "https://github.com/tdykstra" },
						{ name: "BillWagner", url: "https://github.com/BillWagner" },
						{ name: "BenjaminMichaelis", url: "https://github.com/BenjaminMichaelis" },
						{ name: "JohyPark", url: "https://github.com/JohyPark" },
						{ name: "Youssef1313", url: "https://github.com/Youssef1313" },
						{ name: "kendrahavens", url: "https://github.com/kendrahavens" },
						{ name: "gewarren", url: "https://github.com/gewarren" },
						{ name: "devlead", url: "https://github.com/devlead" },
						{ name: "nschonni", url: "https://github.com/nschonni" },
						{ name: "mairaw", url: "https://github.com/mairaw" },
						{ name: "Anduin2017", url: "https://github.com/Anduin2017" },
						{ name: "nxtn", url: "https://github.com/nxtn" },
						{ name: "kennethjohnsen", url: "https://github.com/kennethjohnsen" },
						{ name: "nemrism", url: "https://github.com/nemrism" },
						{ name: "charliegdev", url: "https://github.com/charliegdev" },
						{ name: "Mikejo5000", url: "https://github.com/Mikejo5000" },
						{ name: "jinwood", url: "https://github.com/jinwood" },
						{ name: "isaac2004", url: "https://github.com/isaac2004" }
],
		},
		functions:{}
	};
	</script>
	<script src="https://wcpstatic.microsoft.com/mscc/lib/v2/wcp-consent.js"></script>
	<script src="https://js.monitor.azure.com/scripts/c/ms.jsll-3.min.js"></script>
	<script>window.onedsAwa = window.awa; delete window.awa;</script>	
	<script src="/static/third-party/jsll/4.3.4/jsll-4.js"></script>
	<script nomodule src="/static/third-party/bluebird/3.5.0/bluebird.min.js" integrity="sha384-aD4BDeDGeLXLpPK4yKeqtZQa9dv4a/7mQ+4L5vwshIYH1Mc2BrXvHd32iHzYCQy5" crossorigin="anonymous"></script>
	<script nomodule src="/static/third-party/fetch/3.0.0/fetch.umd.min.js" integrity="sha384-EQIXrC5K2+7X8nGgLkB995I0/6jfAvvyG1ieZ+WYGxgJHFMD/alsG9fSDWvzb5Y1" crossorigin="anonymous"></script>
	<script nomodule src="/static/third-party/template/1.4.0/template.min.js" integrity="sha384-1zKzI6ldTVHMU7n0W2HpE/lhHI+UG4D9IIaxbj3kT2UhCWicdTuJkTtnKuu0CQzN" crossorigin="anonymous"></script>
	<script nomodule src="/static/third-party/url/0.5.7/url.min.js" integrity="sha384-vn7xBMtpSTfzaTRWxj0kVq0UcsbBrTOgZ/M1ISHqe1V358elYva+lfiEC+T8jLPc" crossorigin="anonymous"></script>
	<script src="/_themes/docs.theme/master/en-us/_themes/scripts/2c6911d0.index-polyfills.js"></script>

		<script src="/_themes/docs.theme/master/en-us/_themes/scripts/b5997e7d.index-docs.js"></script>
</head>

<body lang="en-us" dir="ltr">
	<div class="header-holder has-default-focus">
		<a href="#main" class="skip-to-main-link has-outline-color-text visually-hidden-until-focused position-fixed has-inner-focus focus-visible top-0 left-0 right-0 padding-xs has-text-centered has-body-background" tabindex="1">Skip to main content</a>
		
		<div hidden id="cookie-consent-holder"></div>
		<!-- liquid-tag banners global -->
		<div id="headerAreaHolder" data-bi-name="header">
<header role="banner" itemscope="itemscope" itemtype="http://schema.org/Organization">
	<div class="nav-bar">
		<div class="nav-bar-brand">
			<a itemprop="url" href="https://www.microsoft.com" aria-label="Microsoft" class="nav-bar-button">
				<div class="nav-bar-logo has-background-image theme-display is-light" role="presentation" aria-hidden="true" itemprop="logo" itemscope="itemscope"></div>
				<div class="nav-bar-logo has-background-image theme-display is-dark is-high-contrast" role="presentation" aria-hidden="true" itemprop="logo" itemscope="itemscope"></div>
			</a>
		</div>
	</div>
	<div class="nav-bar border-top is-hidden-mobile"></div>
</header>		</div>

						<div class="content-header uhf-container has-padding has-default-focus border-bottom-none" data-bi-name="content-header">
					<nav class="breadcrumb-holder has-padding-none has-padding-left-medium-tablet has-padding-right-medium-tablet has-padding-left-none-uhf-tablet has-padding-left-none-uhf-tablet has-padding-none-desktop flex-grow-1" data-bi-name="breadcrumb" itemscope itemtype="http://schema.org/BreadcrumbList" role="navigation" aria-label="Breadcrumb">
						<ul id="page-breadcrumbs" class="breadcrumbs">
						</ul>
					</nav>
				<div class="content-header-controls">
					<button type="button" class="contents-button button" data-bi-name="contents-expand" aria-haspopup="true">
						<span class="icon"><span class="docon docon-menu" aria-hidden="true"></span></span>
						<span class="contents-expand-title">Contents</span>
					</button>
					<button type="button" class="ap-collapse-behavior ap-expanded button" data-bi-name="ap-collapse" aria-controls="action-panel">
						<span class="icon"><span class="docon docon-exit-mode" aria-hidden="true"></span></span>
						<span>Exit focus mode</span>
					</button>
				</div>
				<div class="has-padding-none-tablet padding-xs font-size-s display-flex justify-content-space-between flex-grow-1 page-action-holder">
					<ul class="is-hidden-mobile action-list justify-content-flex-start has-flex-justify-content-end-tablet display-flex flex-wrap-wrap flex-grow-1 is-unstyled">
						<li hidden>
							<a id="lang-link" class="button is-text has-inner-focus is-small is-icon-only-touch" title="Read in English" data-bi-name="language-toggle">
								<span id="lang-link-icon" class="icon docon docon-locale-globe" aria-hidden="true"></span>
								<span id="lang-link-text" class="is-visually-hidden-touch is-hidden-portrait"></span>
							</a>
						</li>
						<li>
							<button type="button" class="collection button is-text has-inner-focus is-small is-icon-only-touch" data-list-type="collection" data-bi-name="collection" title="Add to collection">
								<span class="icon" aria-hidden="true">
									<span class="docon docon-circle-addition has-text-primary"></span>
								</span>
								<span class="collection-status is-visually-hidden-touch is-hidden-portrait">Save</span>
							</button>
						</li>
							<li id="feedback-section-link">
								<a href="#feedback" class="button is-text has-inner-focus is-small is-icon-only-touch" data-bi-name="comments" title="Send feedback about this page">
									<span class="icon" aria-hidden="true">
										<span class="docon docon-comment-lines"></span>
									</span>
									<span class="is-visually-hidden-touch is-hidden-portrait">Feedback</span>
								</a>
							</li>
								<li id="contenteditbtn">
									<a href="https://github.com/dotnet/docs/blob/main/docs/core/tutorials/with-visual-studio-code.md" class="button is-text has-inner-focus is-icon-only-touch is-small" title="Edit This Document" data-bi-name="edit" data-original_content_git_url="https://github.com/dotnet/docs/blob/live/docs/core/tutorials/with-visual-studio-code.md" data-original_content_git_url_template="{repo}/blob/{branch}/docs/core/tutorials/with-visual-studio-code.md" data-pr_repo="" data-pr_branch="">
									<span class="icon" aria-hidden="true">
										<span class="docon docon-edit-outline"></span>
									</span>
									<span class="is-visually-hidden-touch is-hidden-portrait">Edit</span>
								</a>
							</li>
						<li>
<div class="sharing dropdown has-caret">
	<button class="dropdown-trigger button is-text is-fullwidth justify-content-flex-start has-inner-focus is-small is-icon-only-touch" aria-controls="sharing-menu" aria-expanded="false" title="Share This Document" data-bi-name="share">
		<span class="icon" aria-hidden="true">
			<span class="docon docon-sharing"></span>
		</span>
		<span class="is-visually-hidden-touch is-hidden-portrait">Share</span>
	</button>
	<div class="dropdown-menu has-padding-small" id="sharing-menu">
		<ul data-bi-name="share-links">
			<li>
				<a class="button is-text is-fullwidth justify-content-flex-start has-inner-focus is-small share-twitter" data-bi-name="twitter">
					<span class="icon">
						<span class="docon docon-brand-twitter has-text-primary" aria-hidden="true"></span>
					</span>
					<span>Twitter</span>
				</a>
			</li>
			<li>
				<a class="button is-text is-fullwidth justify-content-flex-start has-inner-focus is-small share-linkedin" data-bi-name="linkedin">
					<span class="icon">
						<span class="docon docon-brand-linkedin has-text-primary" aria-hidden="true"></span>
					</span>
					<span>LinkedIn</span>
				</a>
			</li>
			<li>
				<a class="button is-text is-fullwidth justify-content-flex-start has-inner-focus is-small share-facebook" data-bi-name="facebook">
					<span class="icon">
						<span class="docon docon-brand-facebook has-text-primary" aria-hidden="true"></span>
					</span>
					<span>Facebook</span>
				</a>
			</li>
			<li>
				<a class="button is-text is-fullwidth justify-content-flex-start has-inner-focus is-small share-email" data-bi-name="email">
					<span class="icon">
						<span class="docon docon-mail-message-fill has-text-primary" aria-hidden="true"></span>
					</span>
					<span>Email</span>
				</a>
			</li>
		</ul>
	</div>
</div>						</li>
					</ul>
					<button type="button" class="border contents-button button is-small is-text is-hidden-tablet has-inner-focus" aria-label="Contents" data-bi-name="contents-expand">
						<span class="icon">
							<span class="docon docon-editor-list-bullet" aria-hidden="true"></span>
						</span>
						<span class="contents-expand-title">Table of contents</span>
					</button>
					<div class="is-invisible"></div>
					<div class="is-hidden-tablet level-item is-flexible level-right">
						<button type="button" class="page-actions-button button is-small is-text is-hidden-tablet has-inner-focus border is-full-height  has-margin-left-small" aria-label="Page Actions" data-bi-name="pageactions">
							<span class="icon">
								<span class="docon docon-more-vertical" aria-hidden="true"></span>
							</span>
						</button>
					</div>
				</div>
			</div>



		<div id="disclaimer-holder" class="has-overflow-hidden has-default-focus">
			<!-- liquid-tag banners sectional -->
		</div>
	</div>

	<div class="mainContainer  uhf-container has-top-padding  has-default-focus" data-bi-name="body">

		<div class="columns has-large-gaps is-gapless-mobile ">

			<div id="left-container" class="left-container is-hidden-mobile column is-one-third-tablet is-one-quarter-desktop">
				<nav id="affixed-left-container" class="position-fixed display-flex flex-direction-column" role="navigation" aria-label="Primary"></nav>
			</div>

			<!-- .primary-holder -->
			<section class="primary-holder column is-two-thirds-tablet is-three-quarters-desktop">
				<!--div.columns -->
				<div class="columns is-gapless-mobile has-large-gaps ">


					<div id="main-column" class="column  is-full is-four-fifths-desktop ">

						<main id="main" role="main" class="content " data-bi-name="content" lang="en-us" dir="ltr">



							<h1 id="tutorial-create-a-net-console-application-using-visual-studio-code">Tutorial: Create a .NET console application using Visual Studio Code</h1>

								<ul class="metadata page-metadata" data-bi-name="page info" lang="en-us" dir="ltr">
									<li>
										<time class="is-invisible" data-article-date aria-label="Article review date" datetime="2020-11-17T00:00:00.000Z" data-article-date-source="ms.date">11/17/2020</time>
									</li>
											<li class="readingTime">3 minutes to read</li>
										<li class="contributors-holder">
											<ul class="facepile has-margin-left-none is-small" data-bi-name="contributors">
																<li class="facepile-item">
																	<a href="https://github.com/tdykstra" title="tdykstra" aria-label="tdykstraGithub profile" data-src="https://github.com/tdykstra.png?size=32" data-contributor-name="tdykstra" class="facepile-item-coin"
																	>
																		<img class="facepile-item-coin-image durable-image" aria-hidden="true" src="https://github.com/tdykstra.png?size=32" role="presentation" onerror="this.className='facepile-item-coin-image durable-image has-error';"/>
																		<span class="facepile-item-coin-text durable-image-fallback facepile-item-teal"aria-hidden="true">t</span>
																	</a>
																</li>
																<li class="facepile-item">
																	<a href="https://github.com/BillWagner" title="BillWagner" aria-label="BillWagnerGithub profile" data-src="https://github.com/BillWagner.png?size=32" data-contributor-name="BillWagner" class="facepile-item-coin"
																	>
																		<img class="facepile-item-coin-image durable-image" aria-hidden="true" src="https://github.com/BillWagner.png?size=32" role="presentation" onerror="this.className='facepile-item-coin-image durable-image has-error';"/>
																		<span class="facepile-item-coin-text durable-image-fallback facepile-item-red"aria-hidden="true">B</span>
																	</a>
																</li>
																<li class="facepile-item">
																	<a href="https://github.com/BenjaminMichaelis" title="BenjaminMichaelis" aria-label="BenjaminMichaelisGithub profile" data-src="https://github.com/BenjaminMichaelis.png?size=32" data-contributor-name="BenjaminMichaelis" class="facepile-item-coin"
																	>
																		<img class="facepile-item-coin-image durable-image" aria-hidden="true" src="https://github.com/BenjaminMichaelis.png?size=32" role="presentation" onerror="this.className='facepile-item-coin-image durable-image has-error';"/>
																		<span class="facepile-item-coin-text durable-image-fallback facepile-item-blue"aria-hidden="true">B</span>
																	</a>
																</li>
																<li class="facepile-item">
																	<a href="https://github.com/JohyPark" title="JohyPark" aria-label="JohyParkGithub profile" data-src="https://github.com/JohyPark.png?size=32" data-contributor-name="JohyPark" class="facepile-item-coin"
																	>
																		<img class="facepile-item-coin-image durable-image" aria-hidden="true" src="https://github.com/JohyPark.png?size=32" role="presentation" onerror="this.className='facepile-item-coin-image durable-image has-error';"/>
																		<span class="facepile-item-coin-text durable-image-fallback facepile-item-teal"aria-hidden="true">J</span>
																	</a>
																</li>
																<li class="facepile-item">
																	<a href="https://github.com/Youssef1313" title="Youssef1313" aria-label="Youssef1313Github profile" data-src="https://github.com/Youssef1313.png?size=32" data-contributor-name="Youssef1313" class="facepile-item-coin"
																	>
																		<img class="facepile-item-coin-image durable-image" aria-hidden="true" src="https://github.com/Youssef1313.png?size=32" role="presentation" onerror="this.className='facepile-item-coin-image durable-image has-error';"/>
																		<span class="facepile-item-coin-text durable-image-fallback facepile-item-red"aria-hidden="true">Y</span>
																	</a>
																</li>
													<li class="facepile-item">
															<button aria-label="View all contributors" class="facepile-item-more" title="View all contributors">
																<div class="facepile-item-coin" aria-hidden="true">
																	<span class="facepile-item-coin-text" aria-hidden="true">
																		+13
																	</span>
																</div>
															</button>
													</li>
											</ul>
										</li>
								</ul>

								<nav id="center-doc-outline" class="doc-outline is-hidden-desktop" data-bi-name="intopic toc" role="navigation" aria-label="Article Outline">
									<h3>In this article</h3>
								</nav>


							<!-- <content> -->
								<p>This tutorial shows how to create and run a .NET console application by using Visual Studio Code and the .NET CLI. Project tasks, such as creating, compiling, and running a project are done by using the .NET CLI. You can follow this tutorial with a different code editor and run commands in a terminal if you prefer.</p>
<h2 id="prerequisites">Prerequisites</h2>
<ol>
<li><a href="https://code.visualstudio.com/" data-linktype="external">Visual Studio Code</a> with the <a href="https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp" data-linktype="external">C# extension</a> installed. For information about how to install extensions on Visual Studio Code, see <a href="https://code.visualstudio.com/docs/editor/extension-gallery" data-linktype="external">VS Code Extension Marketplace</a>.</li>
<li>The <a href="https://dotnet.microsoft.com/download" data-linktype="external">.NET 5.0 SDK or later</a></li>
</ol>
<h2 id="create-the-app">Create the app</h2>
<p>Create a .NET console app project named &quot;HelloWorld&quot;.</p>
<ol>
<li><p>Start Visual Studio Code.</p>
</li>
<li><p>Select <strong>File</strong> &gt; <strong>Open Folder</strong> (<strong>File</strong> &gt; <strong>Open...</strong> on macOS) from the main menu.</p>
</li>
<li><p>In the <strong>Open Folder</strong> dialog, create a <em>HelloWorld</em> folder and click <strong>Select Folder</strong> (<strong>Open</strong> on macOS).</p>
<p>The folder name becomes the project name and the namespace name by default. You'll add code later in the tutorial that assumes the project namespace is <code>HelloWorld</code>.</p>
</li>
<li><p>Open the <strong>Terminal</strong> in Visual Studio Code by selecting <strong>View</strong> &gt; <strong>Terminal</strong> from the main menu.</p>
<p>The <strong>Terminal</strong> opens with the command prompt in the <em>HelloWorld</em> folder.</p>
</li>
<li><p>In the <strong>Terminal</strong>, enter the following command:</p>
<pre><code class="lang-dotnetcli">dotnet new console
</code></pre>
</li>
</ol>
<p>The template creates a simple &quot;Hello World&quot; application. It calls the <a href="/en-us/dotnet/api/system.console.writeline#System_Console_WriteLine_System_String_" data-linktype="absolute-path">Console.WriteLine(String)</a> method to display &quot;Hello World!&quot; in the console window.</p>
<p>The template code defines a class, <code>Program</code>, with a single method, <code>Main</code>, that takes a <a href="/en-us/dotnet/api/system.string" data-linktype="absolute-path">String</a> array as an argument:</p>
<pre><code class="lang-csharp">using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(&quot;Hello World!&quot;);
        }
    }
}
</code></pre>
<p><code>Main</code> is the application entry point, the method that's called automatically by the runtime when it launches the application. Any command-line arguments supplied when the application is launched are available in the <em>args</em> array.</p>
<h2 id="run-the-app">Run the app</h2>
<p>Run the following command in the <strong>Terminal</strong>:</p>
<pre><code class="lang-dotnetcli">dotnet run
</code></pre>
<p>The program displays &quot;Hello World!&quot; and ends.</p>
<p><img src="media/with-visual-studio-code/dotnet-run-command.png" alt="The dotnet run command" data-linktype="relative-path"/></p>
<h2 id="enhance-the-app">Enhance the app</h2>
<p>Enhance the application to prompt the user for their name and display it along with the date and time.</p>
<ol>
<li><p>Open <em>Program.cs</em> by clicking on it.</p>
<p>The first time you open a C# file in Visual Studio Code, <a href="https://www.omnisharp.net/" data-linktype="external">OmniSharp</a> loads in the editor.</p>
<p><img src="media/with-visual-studio-code/open-program-cs.png" alt="Open the Program.cs file" data-linktype="relative-path"/></p>
</li>
<li><p>Select <strong>Yes</strong> when Visual Studio Code prompts you to add the missing assets to build and debug your app.</p>
<p><img src="media/with-visual-studio-code/missing-assets.png" alt="Prompt for missing assets" data-linktype="relative-path"/></p>
</li>
<li><p>Replace the contents of the <code>Main</code> method in <em>Program.cs</em>, which is the line that calls <code>Console.WriteLine</code>, with the following code:</p>
<pre>
<code class="lang-csharp">Console.WriteLine(&quot;What is your name?&quot;);
var name = Console.ReadLine();
var currentDate = DateTime.Now;
Console.WriteLine($&quot;{Environment.NewLine}Hello, {name}, on {currentDate:d} at {currentDate:t}!&quot;);
Console.Write($&quot;{Environment.NewLine}Press any key to exit...&quot;);
Console.ReadKey(true);
</code></pre>
<p>This code displays a prompt in the console window and waits until the user enters a string followed by the <kbd>Enter</kbd> key. It stores this string in a variable named <code>name</code>. It also retrieves the value of the <a href="/en-us/dotnet/api/system.datetime.now#System_DateTime_Now" data-linktype="absolute-path">DateTime.Now</a> property, which contains the current local time, and assigns it to a variable named <code>date</code>. And it displays these values in the console window. Finally, it displays a prompt in the console window and calls the <a href="/en-us/dotnet/api/system.console.readkey#System_Console_ReadKey_System_Boolean_" data-linktype="absolute-path">Console.ReadKey(Boolean)</a> method to wait for user input.</p>
<p><a href="/en-us/dotnet/api/system.environment.newline#System_Environment_NewLine" data-linktype="absolute-path">NewLine</a> is a platform-independent and language-independent way to represent a line break. Alternatives are <code>\n</code> in C# and <code>vbCrLf</code> in Visual Basic.</p>
<p>The dollar sign (<code>$</code>) in front of a string lets you put expressions such as variable names in curly braces in the string. The expression value is inserted into the string in place of the expression. This syntax is referred to as <a href="../../csharp/language-reference/tokens/interpolated" data-linktype="relative-path">interpolated strings</a>.</p>
</li>
<li><p>Save your changes.</p>
<div class="IMPORTANT">
<p>Important</p>
<p>In Visual Studio Code, you have to explicitly save changes. Unlike Visual Studio, file changes are not automatically saved when you build and run an app.</p>
</div>
</li>
<li><p>Run the program again:</p>
<pre><code class="lang-dotnetcli">dotnet run
</code></pre>
</li>
<li><p>Respond to the prompt by entering a name and pressing the <kbd>Enter</kbd> key.</p>
<p><span class="mx-imgBorder">
<img src="media/debugging-with-visual-studio-code/run-modified-program.png" alt="Terminal window with modified program output" data-linktype="relative-path">
</span>
</p>
</li>
<li><p>Press any key to exit the program.</p>
</li>
</ol>
<h2 id="additional-resources">Additional resources</h2>
<ul>
<li><a href="https://code.visualstudio.com/docs/setup/setup-overview" data-linktype="external">Setting up Visual Studio Code</a></li>
</ul>
<h2 id="next-steps">Next steps</h2>
<p>In this tutorial, you created a .NET console application. In the next tutorial, you debug the app.</p>
<div class="nextstepaction">
<p><a href="debugging-with-visual-studio-code" data-linktype="relative-path">Debug a .NET console application using Visual Studio Code</a></p>
</div>

							<!-- </content> -->

						</main>

						<!-- page rating section -->
								<div class="is-hidden-desktop border-top has-margin-top-large has-padding-top-large binary-rating-holder">
									
	
	

	<div class="feedback-verbatim border-bottom has-padding-bottom-large has-margin-bottom-small" data-bi-name="rating">
    <div class="binary-rating">
        <div class="binary-rating-buttons">
				<h3 class="font-weight-semibold has-margin-top-none font-size-h4 margin-bottom-xs">Is this page helpful?</h3>
			<div>
                <button class="thumb-rating like has-inner-focus" title="Yes" data-bi-name="rating-yes" aria-expanded="false" data-bi-sat="1" aria-controls="rating-container-desktop">
                    <span aria-hidden="true" class="icon docon docon-like"></span>
                    <span>Yes</span>
                </button>
                <button class="thumb-rating dislike has-inner-focus" title="No" data-bi-name="rating-no" data-bi-sat="0" aria-expanded="false" aria-controls="rating-container-desktop">
                    <span aria-hidden="true" class="icon docon docon-dislike"></span>
                    <span>No</span>
                </button>
            </div>
        </div>
        <form class="feedback-verbatim-form is-hidden" id="rating-container-desktop">
            <div class="verbatim-textarea box position-relative box-shadow-none border has-margin-top-small has-padding-extra-small font-size-xs">
                <label for="rating-textarea-desktop" class="visually-hidden">Any additional feedback?</label>
                <textarea id="rating-textarea-desktop" rows="4" maxlength="999" placeholder="Any additional feedback?" required class="textarea border-none box-shadow-none has-inner-focus"></textarea>
		    </div>
			<p class="font-size-xs has-line-height-reset">Feedback will be sent to Microsoft: By pressing the submit button, your feedback will be used to improve Microsoft products and services. <a href="https://privacy.microsoft.com/en-us/privacystatement">Privacy policy.</a></p>
            <div class="buttons is-right margin-top-xs has-margin-right-extra-small">
                <button class="skip-rating button is-transparent has-text-primary is-small border-none" type="button">Skip</button>
                <button class="submit-rating button is-primary is-small" data-bi-name="rating-verbatim" disabled type="submit">Submit</button>
            </div>
        </form>
    </div>
    <div class="thankyou-rating is-hidden" tabindex="-1">
        <p>Thank you.</p>
    </div>
</div>									</div>
						<!-- end page rating section -->


						<!-- recommendations section -->
							<section id="recommendations-section" data-bi-name="recommendations"></section>
						<!-- end recommendations section -->

						<!-- feedback section -->
<section class="feedback-section position-relative" data-bi-name="feedback-section">

    <h2 id="feedback" class="title is-3 has-margin-top-large">Feedback</h2>

    <div class="alert choose-feedback-type">
        <p aria-hidden="true" id="send-feedback-about">Submit and view feedback for</p>

        <div class="choose-feedback-buttons margin-top-xs">
                <a class="button has-external-link-indicator feedback-type-product has-margin-bottom-small" aria-label="Send feedback about this product" href="https://aka.ms/feedback/report?space=61" data-bi-name="product-feedback">
                    <span>This product</span>
                </a>

			<a class="button feedback-type-product has-margin-bottom-small github-link" aria-label="Send feedback about this page" data-bi-name="create-issue-on-github">
				<span aria-hidden="true" class="docon docon-brand-github has-padding-right-extra-small"></span>
				<span>This page</span>
			</a>
        </div>
    </div>

    <div class="action-container display-flex justify-content-flex-end has-margin-top-small has-margin-bottom-small">
        <a class="view-on-github has-external-link-indicator" data-bi-name="view-on-github" href="https://github.com/dotnet/docs/issues">
            <span aria-hidden="true" class="docon docon-brand-github"></span>
            <span>View all page feedback</span>
        </a>
    </div>
</section>
						<!-- end feedback section -->

						<!-- feedback report section -->
						<!-- end feedback report section -->

						<div class="border-top is-visible-interactive has-default-focus has-margin-top-large ">



	<footer id="footer-interactive" data-bi-name="footer" class="footer-layout">
	<div class="display-flex is-full-height has-padding-right-extra-large-desktop">
			<a data-mscc-ic="false" class="locale-selector-link flex-shrink-0" href="#" data-bi-name="select-locale"><span class="icon docon docon-world font-size-l has-margin-right-small" aria-hidden="true"></span><span class="local-selector-link-text"></span></a>
		<div class="margin-inline-xs flex-shrink-0">
<div class="dropdown has-caret-up">
	<button class="dropdown-trigger button is-transparent is-small is-icon-only-touch has-inner-focus theme-dropdown-trigger"
		aria-controls="theme-menu-interactive" aria-expanded="false" title="Theme" data-bi-name="theme">
		<span class="icon">
			<span class="docon docon-sun" aria-hidden="true"></span>
		</span>
		<span>Theme</span>
	</button>
	<div class="dropdown-menu" id="theme-menu-interactive" role="menu">
		<ul class="theme-selector has-padding-small">
			<li class="theme is-block">
				<button class="button is-text is-small theme-control is-fullwidth justify-content-flex-start"
					data-theme-to="light">
					<span class="theme-light has-margin-right-small">
						<span
							class="theme-selector-icon css-variable-support border is-inline-block has-body-background"
							aria-hidden="true">
							<svg class="svg" xmlns="http://www.w3.org/2000/svg"
								viewBox="0 0 22 14">
								<rect width="22" height="14" class="has-fill-body-background" />
								<rect x="5" y="5" width="12" height="4" class="has-fill-secondary" />
								<rect x="5" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="8" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="11" y="2" width="3" height="1" class="has-fill-secondary" />
								<rect x="1" y="1" width="2" height="2" class="has-fill-secondary" />
								<rect x="5" y="10" width="7" height="2" rx="0.3" class="has-fill-primary" />
								<rect x="19" y="1" width="2" height="2" rx="1" class="has-fill-secondary" />
							</svg>
						</span>
					</span>
					<span role="menuitem">
Light					</span>
				</button>
			</li>
			<li class="theme is-block">
				<button class="button is-text is-small theme-control is-fullwidth justify-content-flex-start"
					data-theme-to="dark">
					<span class="theme-dark has-margin-right-small">
						<span
							class="border theme-selector-icon css-variable-support is-inline-block has-body-background"
							aria-hidden="true">
							<svg class="svg" xmlns="http://www.w3.org/2000/svg"
								viewBox="0 0 22 14">
								<rect width="22" height="14" class="has-fill-body-background" />
								<rect x="5" y="5" width="12" height="4" class="has-fill-secondary" />
								<rect x="5" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="8" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="11" y="2" width="3" height="1" class="has-fill-secondary" />
								<rect x="1" y="1" width="2" height="2" class="has-fill-secondary" />
								<rect x="5" y="10" width="7" height="2" rx="0.3" class="has-fill-primary" />
								<rect x="19" y="1" width="2" height="2" rx="1" class="has-fill-secondary" />
							</svg>
						</span>
					</span>
					<span role="menuitem">
Dark					</span>
				</button>
			</li>
			<li class="theme is-block">
				<button class="button is-text is-small theme-control is-fullwidth justify-content-flex-start"
					data-theme-to="high-contrast">
					<span class="theme-high-contrast has-margin-right-small">
						<span
							class="border theme-selector-icon css-variable-support is-inline-block has-body-background"
							aria-hidden="true">
							<svg class="svg" xmlns="http://www.w3.org/2000/svg"
								viewBox="0 0 22 14">
								<rect width="22" height="14" class="has-fill-body-background" />
								<rect x="5" y="5" width="12" height="4" class="has-fill-secondary" />
								<rect x="5" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="8" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="11" y="2" width="3" height="1" class="has-fill-secondary" />
								<rect x="1" y="1" width="2" height="2" class="has-fill-secondary" />
								<rect x="5" y="10" width="7" height="2" rx="0.3" class="has-fill-primary" />
								<rect x="19" y="1" width="2" height="2" rx="1" class="has-fill-secondary" />
							</svg>
						</span>
					</span>
					<span role="menuitem">
High contrast					</span>
				</button>
			</li>
		</ul>
	</div>
</div>		</div>
	</div>
	<ul class="links" data-bi-name="footerlinks">
		<li class="manage-cookies-holder" hidden></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/previous-versions/" data-bi-name="archivelink">Previous Version Docs</a></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/teamblog" data-bi-name="bloglink">Blog</a></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/contribute" data-bi-name="contributorGuide">Contribute</a></li>
					<li><a data-mscc-ic="false" href="https://go.microsoft.com/fwlink/?LinkId=521839" data-bi-name="privacy">Privacy &amp; Cookies</a></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/legal/termsofuse" data-bi-name="termsofuse">Terms of Use</a></li>
				<li><a data-mscc-ic="false" href="https://www.microsoft.com/en-us/legal/intellectualproperty/Trademarks/EN-US.aspx" data-bi-name="trademarks">Trademarks</a></li>
		<li>&copy; Microsoft 2021</li>
	</ul>
</footer>
						</div>
					</div>
					
						<div class="font-size-s right-container column is-one-quarter is-one-fifth-desktop is-hidden-mobile is-hidden-tablet-only" data-bi-name="pageactions" role="complementary" aria-label="Page Actions">
							<div id="affixed-right-container" class="doc-outline position-fixed is-vertically-scrollable">
									
	
	

	<div class="feedback-verbatim border-bottom has-padding-bottom-small has-margin-bottom-small" data-bi-name="rating">
    <div class="binary-rating">
        <div class="binary-rating-buttons">

				<h3 class="font-weight-semibold has-margin-top-none has-margin-bottom-small">Is this page helpful?</h3>
			<div>
                <button class="thumb-rating like has-inner-focus" title="Yes" data-bi-name="rating-yes" aria-expanded="false" data-bi-sat="1" aria-controls="rating-container-mobile">
                    <span aria-hidden="true" class="icon docon docon-like"></span>
                    <span>Yes</span>
                </button>
                <button class="thumb-rating dislike has-inner-focus" title="No" data-bi-name="rating-no" data-bi-sat="0" aria-expanded="false" aria-controls="rating-container-mobile">
                    <span aria-hidden="true" class="icon docon docon-dislike"></span>
                    <span>No</span>
                </button>
            </div>
        </div>
        <form class="feedback-verbatim-form is-hidden" id="rating-container-mobile">
            <div class="verbatim-textarea box position-relative box-shadow-none border has-margin-top-small has-padding-extra-small font-size-xs">
                <label for="rating-textarea-mobile" class="visually-hidden">Any additional feedback?</label>
                <textarea id="rating-textarea-mobile" rows="4" maxlength="999" placeholder="Any additional feedback?" required class="textarea border-none box-shadow-none has-inner-focus"></textarea>
		    </div>
			<p class="font-size-xs has-line-height-reset">Feedback will be sent to Microsoft: By pressing the submit button, your feedback will be used to improve Microsoft products and services. <a href="https://privacy.microsoft.com/en-us/privacystatement">Privacy policy.</a></p>
            <div class="buttons is-right margin-top-xs has-margin-right-extra-small">
                <button class="skip-rating button is-transparent has-text-primary is-small border-none" type="button">Skip</button>
                <button class="submit-rating button is-primary is-small" data-bi-name="rating-verbatim" disabled type="submit">Submit</button>
            </div>
        </form>
    </div>
    <div class="thankyou-rating is-hidden" tabindex="-1">
        <p>Thank you.</p>
    </div>
</div>								<nav id="side-doc-outline" data-bi-name="intopic toc" role="navigation" aria-label="Article Outline">
									<h3>In this article</h3>
								</nav>
							</div>
						</div>

				</div>
				<!--end of div.columns -->

			</section>
			<!--end of .primary-holder -->

			<!-- interactive container -->
			<aside id="interactive-container" class="interactive-container is-visible-interactive column has-body-background-dark ">
			</aside>
			<!-- end of interactive container -->
		</div>

	</div>
	<!--end of .mainContainer -->

	<section class="border-top has-default-focus is-hidden-interactive has-margin-top-large ">



	<footer id="footer" data-bi-name="footer" class="footer-layout uhf-container has-padding" role="contentinfo">
	<div class="display-flex is-full-height has-padding-right-extra-large-desktop">
			<a data-mscc-ic="false" class="locale-selector-link flex-shrink-0" href="#" data-bi-name="select-locale"><span class="icon docon docon-world font-size-l has-margin-right-small" aria-hidden="true"></span><span class="local-selector-link-text"></span></a>
		<div class="margin-inline-xs flex-shrink-0">
<div class="dropdown has-caret-up">
	<button class="dropdown-trigger button is-transparent is-small is-icon-only-touch has-inner-focus theme-dropdown-trigger"
		aria-controls="theme-menu" aria-expanded="false" title="Theme" data-bi-name="theme">
		<span class="icon">
			<span class="docon docon-sun" aria-hidden="true"></span>
		</span>
		<span>Theme</span>
	</button>
	<div class="dropdown-menu" id="theme-menu" role="menu">
		<ul class="theme-selector has-padding-small">
			<li class="theme is-block">
				<button class="button is-text is-small theme-control is-fullwidth justify-content-flex-start"
					data-theme-to="light">
					<span class="theme-light has-margin-right-small">
						<span
							class="theme-selector-icon css-variable-support border is-inline-block has-body-background"
							aria-hidden="true">
							<svg class="svg" xmlns="http://www.w3.org/2000/svg"
								viewBox="0 0 22 14">
								<rect width="22" height="14" class="has-fill-body-background" />
								<rect x="5" y="5" width="12" height="4" class="has-fill-secondary" />
								<rect x="5" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="8" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="11" y="2" width="3" height="1" class="has-fill-secondary" />
								<rect x="1" y="1" width="2" height="2" class="has-fill-secondary" />
								<rect x="5" y="10" width="7" height="2" rx="0.3" class="has-fill-primary" />
								<rect x="19" y="1" width="2" height="2" rx="1" class="has-fill-secondary" />
							</svg>
						</span>
					</span>
					<span role="menuitem">
Light					</span>
				</button>
			</li>
			<li class="theme is-block">
				<button class="button is-text is-small theme-control is-fullwidth justify-content-flex-start"
					data-theme-to="dark">
					<span class="theme-dark has-margin-right-small">
						<span
							class="border theme-selector-icon css-variable-support is-inline-block has-body-background"
							aria-hidden="true">
							<svg class="svg" xmlns="http://www.w3.org/2000/svg"
								viewBox="0 0 22 14">
								<rect width="22" height="14" class="has-fill-body-background" />
								<rect x="5" y="5" width="12" height="4" class="has-fill-secondary" />
								<rect x="5" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="8" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="11" y="2" width="3" height="1" class="has-fill-secondary" />
								<rect x="1" y="1" width="2" height="2" class="has-fill-secondary" />
								<rect x="5" y="10" width="7" height="2" rx="0.3" class="has-fill-primary" />
								<rect x="19" y="1" width="2" height="2" rx="1" class="has-fill-secondary" />
							</svg>
						</span>
					</span>
					<span role="menuitem">
Dark					</span>
				</button>
			</li>
			<li class="theme is-block">
				<button class="button is-text is-small theme-control is-fullwidth justify-content-flex-start"
					data-theme-to="high-contrast">
					<span class="theme-high-contrast has-margin-right-small">
						<span
							class="border theme-selector-icon css-variable-support is-inline-block has-body-background"
							aria-hidden="true">
							<svg class="svg" xmlns="http://www.w3.org/2000/svg"
								viewBox="0 0 22 14">
								<rect width="22" height="14" class="has-fill-body-background" />
								<rect x="5" y="5" width="12" height="4" class="has-fill-secondary" />
								<rect x="5" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="8" y="2" width="2" height="1" class="has-fill-secondary" />
								<rect x="11" y="2" width="3" height="1" class="has-fill-secondary" />
								<rect x="1" y="1" width="2" height="2" class="has-fill-secondary" />
								<rect x="5" y="10" width="7" height="2" rx="0.3" class="has-fill-primary" />
								<rect x="19" y="1" width="2" height="2" rx="1" class="has-fill-secondary" />
							</svg>
						</span>
					</span>
					<span role="menuitem">
High contrast					</span>
				</button>
			</li>
		</ul>
	</div>
</div>		</div>
	</div>
	<ul class="links" data-bi-name="footerlinks">
		<li class="manage-cookies-holder" hidden></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/previous-versions/" data-bi-name="archivelink">Previous Version Docs</a></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/teamblog" data-bi-name="bloglink">Blog</a></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/contribute" data-bi-name="contributorGuide">Contribute</a></li>
					<li><a data-mscc-ic="false" href="https://go.microsoft.com/fwlink/?LinkId=521839" data-bi-name="privacy">Privacy &amp; Cookies</a></li>
				<li><a data-mscc-ic="false" href="https://docs.microsoft.com/en-us/legal/termsofuse" data-bi-name="termsofuse">Terms of Use</a></li>
				<li><a data-mscc-ic="false" href="https://www.microsoft.com/en-us/legal/intellectualproperty/Trademarks/EN-US.aspx" data-bi-name="trademarks">Trademarks</a></li>
		<li>&copy; Microsoft 2021</li>
	</ul>
</footer>
	</section>

		<script type="text/x-mathjax-config">
			MathJax.Hub.Config({
				showMathMenu: false,
				showMathMenuMSIE: false,
				tex2jax: {
					inlineMath: [['$','$'], ['\\(','\\)']],
					processEscapes: true
				}
			});
			MathJax.Hub.Register.StartupHook("End", function () {
				document.documentElement.classList.add('mathjax-complete');
			});
		</script>
		<script src="/static/third-party/MathJax/2.7.2/MathJax.js?config=TeX-AMS_CHTML" integrity="sha384-RLsAi7wiVvnmHrRjlVvUjU45C0bfsIBg6Gsxue6azjJi+lA5q5uK+XbGzO3yn5g1" crossorigin="anonymous"></script>
	<div id="action-panel" role="region" aria-label="Action Panel" class="action-panel has-default-focus" tabindex="-1"></div>
</body>
</html>
