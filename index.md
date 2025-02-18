---
layout: default
lead: WebAssembly or <i>wasm</i> is a new portable, size- and load-time-efficient format suitable for compilation to the web.
---
<div class="flash flash-warn flash-messages">
  WebAssembly is currently being designed as an open standard by a <a href="https://www.w3.org/community/webassembly/">W3C Community Group</a> that includes representatives from all major browsers. Expect the contents of this website and its associated design repositories to be in flux: everything is still under discussion and subject to change.
</div>
<h2>Overview</h2>
<ul>
  <li>
    <p><strong>Efficient and fast</strong>: The wasm <a href="https://github.com/WebAssembly/design/blob/master/Semantics.md">stack machine</a> is designed to be encoded in a size- and load-time-efficient <a href="https://github.com/WebAssembly/design/blob/master/BinaryEncoding.md">binary format</a>. WebAssembly aims to execute at native speed by taking advantage of <a href="https://github.com/WebAssembly/design/blob/master/Portability.md#assumptions-for-efficient-execution">common hardware capabilities</a> available on a wide range of platforms.</p>
  </li>
  <li>
    <p><strong>Safe</strong>: WebAssembly describes a memory-safe, sandboxed <a href="https://github.com/WebAssembly/design/blob/master/Semantics.md#linear-memory">execution environment</a> that may even be implemented inside existing JavaScript virtual machines. When <a href="https://github.com/WebAssembly/design/blob/master/Web.md">embedded in the web</a>, WebAssembly will enforce the same-origin and permissions security policies of the browser.</p>
  </li>
  <li>
    <p><strong>Open and debuggable</strong>: WebAssembly is designed to be pretty-printed in a <a href="https://github.com/WebAssembly/design/blob/master/TextFormat.md">textual format</a> for debugging, testing, experimenting, optimizing, learning, teaching, and writing programs by hand. The textual format will be used when <a href="https://github.com/WebAssembly/design/blob/master/FAQ.md#will-webassembly-support-view-source-on-the-web">viewing the source</a> of wasm modules on
      the web.</p>
  </li>
  <li>
    <p><strong>Part of the open web platform</strong>: WebAssembly is designed to maintain the versionless, feature-tested, and backwards-compatible <a href="https://github.com/WebAssembly/design/blob/master/Web.md">nature of the web</a>. WebAssembly modules will be able to call into and out of the JavaScript context and access browser functionality through the same Web APIs accessible from JavaScript. WebAssembly also supports <a href="https://github.com/WebAssembly/design/blob/master/NonWeb.md">non-web</a> embeddings.</p>
  </li>
</ul>
<p>Read the project's <a href="https://github.com/WebAssembly/design/blob/master/HighLevelGoals.md">high-level goals</a> and consult the <a href="https://github.com/WebAssembly/design/blob/master/FAQ.md">FAQ</a> section for more information.</p>
<h2>Roadmap</h2>
<table>
  <thead>
    <tr>
      <th class="text-left"><a href="https://github.com/WebAssembly/design/blob/master/MVP.md">MVP</a></th>
      <th class="text-left">Soon <a href="https://github.com/WebAssembly/design/blob/master/PostMVP.md">after MVP</a></th>
      <th class="text-left"><a href="https://github.com/WebAssembly/design/blob/master/FutureFeatures.md">Future versions</a></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>asm.js functional parity</td>
      <td>threads</td>
      <td>finer-grained memory control</td>
    </tr>
    <tr>
      <td>validation semantics</td>
      <td>shared memory</td>
      <td>large page support</td>
    </tr>
    <tr>
      <td>execution semantics</td>
      <td>dynamic linking</td>
      <td>more expressive control flow</td>
    </tr>
    <tr>
      <td>module semantics</td>
      <td>zero-cost exceptions</td>
      <td>GC/DOM integration</td>
    </tr>
    <tr>
      <td>binary encoding</td>
      <td>fixed-width SIMD</td>
      <td>linear memory >4GiB</td>
    </tr>
    <tr>
      <td>textual format</td>
      <td></td>
      <td>... and <a href="https://github.com/WebAssembly/design/blob/master/FutureFeatures.md">more</a></td>
    </tr>
    <tr>
      <td>cross-browser support</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>polyfill-able in JS</td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>
<h2>SDK</h2>
<p>For bleeding edge compilation of C/C++ or asm.js to WebAssembly, see the instructions for  <a href="https://github.com/WebAssembly/binaryen">Binaryen</a>, a derivative of <a href="http://kripken.github.io/emscripten-site/">Emscripten</a>.</p>
<h2>Contributing</h2>
<p>The actual WebAssembly specification is being developed in the <a href="https://github.com/WebAssembly/spec/">spec repository</a>. For now, high-level design discussions should continue to be held in the <a href="https://github.com/WebAssembly/design/">design repository</a>, via issues and pull requests, so that the spec work can remain focused.</p>
<p>Join us:</p>
<ul>
  <li>in the <a href="https://www.w3.org/community/webassembly/">W3C Community Group</a></li>
  <li>on IRC: <a href="https://kiwiirc.com/client/irc.w3.org/?nick=wasmer-?#webassembly">irc://irc.w3.org:6667/#webassembly</a></li>
  <li>by <a href="https://github.com/WebAssembly/design/blob/master/Contributing.md">contributing</a>!</li>
</ul>
<p>The WebAssembly <a href="https://wasm-stat.us/console">waterfall</a> builds, executes, and <a href="https://gsdview.appspot.com/wasm-llvm/builds/">archives</a> different components of the WebAssembly project, enabling end-to-end integration tests of LLVM compilation and execution in d8 and the Binaryen interpreter.</p>
<p>When contributing, please follow our <a href="https://github.com/WebAssembly/design/blob/master/CodeOfConduct.md">Code of Ethics and Professional Conduct</a>.</p>


