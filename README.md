Available targets
<dl>
<dt><code>all-srpms</code></dt><dd>Build all SRPMS for all of LLVM's sub-projects.</dd>
<dt><code>srpm-%</code></dt><dd>With "make srpm-PROJECT you can build an SRPM for an individual LLVM<br/>
 sub-project.</dd>
<dt><code>all-rpms</code></dt><dd>Build all of LLVM's sub-projects in the correct order.</dd>
<dt><code>clean</code></dt><dd>Remove the artifacts for all projects.</dd>
<dt><code>clean-%</code></dt><dd>"make clean-PROJECT" to remove the artifacts for an<br/>
 individual project only.</dd>
<dt><code>clean-cache</code></dt><dd>Remove the ./dnf-cache DNF cache directory.<br/>
 NOTE: This might require to be run as root for permission problems.</dd>
<dt><code>container-image</code></dt><dd>Builds the container image that will be used for build SRPMs and RPMs.</dd>
<dt><code>python-lit</code></dt><dd>Build LLVM's python-lit sub-project.</dd>
<dt><code>compat-llvm</code></dt><dd>Build the compatibility packages for LLVM's llvm sub-project.</dd>
<dt><code>compat-clang</code></dt><dd>Build the compatibility packages for LLVM's clang sub-project.</dd>
<dt><code>llvm</code></dt><dd>Build LLVM's llvm sub-project.</dd>
<dt><code>clang</code></dt><dd>Build LLVM's clang sub-project.</dd>
<dt><code>lld</code></dt><dd>Build LLVM's lld sub-project.</dd>
<dt><code>shell-%</code></dt><dd>This mounts a project and with all dependent repos mounted (expecting they<br/>
 exist) and then enter a bash-shell for experiments or rerunning tests and<br/>
 whatnot. To get the container in a good shape, we also install build<br/>
 dependencies as defined in the project's spec file.</dd>
<dt><code>koji-compat</code></dt><dd>Initiate a koji build of compat-llvm and compat-clang using the<br/>
 SRPMs for these packages.<br/>
 NOTE: The SRPMs can be generated using "make all-srpms".</dd>
<dt><code>koji-no-compat</code></dt><dd>Initiate a koji build of python-lit, llvm, clang and lld using the<br/>
 SRPMs for these packages.<br/>
 NOTE: The SRPMs can be generated using "make all-srpms".</dd>
<dt><code>koji-wait-repo-%</code></dt><dd>Waits for 30 minutes on the RPM of the given project to appear in the repo for<br/>
 the build tag.</dd>
<dt><code>koji-%</code></dt><dd>Takes the SRPM for the given project and builds it on koji</dd>
<dt><code>help</code></dt><dd>Display this help text.</dd>
<dt><code>help-html</code></dt><dd>Display this help text as an HTML definition list for better documentation generation</dd>
</dl>
