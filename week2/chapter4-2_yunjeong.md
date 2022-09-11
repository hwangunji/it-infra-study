<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>4.인프라를 지탱하는 기본 이론</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	text-indent: -1.7em;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

.simple-table {
	margin-top: 1em;
	font-size: 0.875rem;
	empty-cells: show;
}
.simple-table td {
	height: 29px;
	min-width: 120px;
}

.simple-table th {
	height: 29px;
	min-width: 120px;
}

.simple-table-header-color {
	background: rgb(247, 246, 243);
	color: black;
}
.simple-table-header {
	font-weight: 500;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	max-height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, ui-serif, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK JP'; }
.pdf:lang(zh-CN) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC'; }
.pdf:lang(zh-TW) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK TC'; }
.pdf:lang(ko-KR) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK KR'; }
.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK JP'; }
.pdf:lang(zh-CN) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK SC'; }
.pdf:lang(zh-TW) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK TC'; }
.pdf:lang(ko-KR) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK KR'; }
.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.highlight-default {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.highlight-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.highlight-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.highlight-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.highlight-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.highlight-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.highlight-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.highlight-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.highlight-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.highlight-gray_background {
	background: rgba(241, 241, 239, 1);
}
.highlight-brown_background {
	background: rgba(244, 238, 238, 1);
}
.highlight-orange_background {
	background: rgba(251, 236, 221, 1);
}
.highlight-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.highlight-teal_background {
	background: rgba(237, 243, 236, 1);
}
.highlight-blue_background {
	background: rgba(231, 243, 248, 1);
}
.highlight-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.highlight-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.highlight-red_background {
	background: rgba(253, 235, 236, 1);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.block-color-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.block-color-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.block-color-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.block-color-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.block-color-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.block-color-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.block-color-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.block-color-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.block-color-gray_background {
	background: rgba(241, 241, 239, 1);
}
.block-color-brown_background {
	background: rgba(244, 238, 238, 1);
}
.block-color-orange_background {
	background: rgba(251, 236, 221, 1);
}
.block-color-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.block-color-teal_background {
	background: rgba(237, 243, 236, 1);
}
.block-color-blue_background {
	background: rgba(231, 243, 248, 1);
}
.block-color-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.block-color-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.block-color-red_background {
	background: rgba(253, 235, 236, 1);
}
.select-value-color-pink { background-color: rgba(245, 224, 233, 1); }
.select-value-color-purple { background-color: rgba(232, 222, 238, 1); }
.select-value-color-green { background-color: rgba(219, 237, 219, 1); }
.select-value-color-gray { background-color: rgba(227, 226, 224, 1); }
.select-value-color-opaquegray { background-color: rgba(255, 255, 255, 0.0375); }
.select-value-color-orange { background-color: rgba(250, 222, 201, 1); }
.select-value-color-brown { background-color: rgba(238, 224, 218, 1); }
.select-value-color-red { background-color: rgba(255, 226, 221, 1); }
.select-value-color-yellow { background-color: rgba(253, 236, 200, 1); }
.select-value-color-blue { background-color: rgba(211, 229, 239, 1); }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="efc7db12-c156-4661-83a1-a9d69baa39f9" class="page sans"><header><div class="page-header-icon undefined"><span class="icon">💡</span></div><h1 class="page-title">4.인프라를 지탱하는 기본 이론</h1></header><div class="page-body"><h2 id="f9c30fa3-f89e-46d0-920f-4d4132484bda" class="">Q1. 직렬과 병렬에 대해서 설명 + 동시성과 병렬성에 대해 설명하세요.</h2><ul id="b8d7861b-68b6-48bc-bb66-37519b8d3c4b" class="bulleted-list"><li style="list-style-type:disc">병렬 : 처리의 효율을 위해 CPU나 스레드를 여러개 이용해서 병렬적으로 처리하는 방법</li></ul><ul id="df872c0b-c93a-486f-91be-4011d14eed59" class="bulleted-list"><li style="list-style-type:disc">동시성<ul id="6caff03e-4f68-4ad7-94a4-4faa672aba5d" class="bulleted-list"><li style="list-style-type:circle"><strong>프로세서 하나</strong>가 이것 조금 저것 조금해서 여러 작업을 돌아가면서 일부분씩 진행하여 마치 동시에 진행되고 있는 것처럼 보이는 것</li></ul><ul id="fa612a49-ac0c-47a1-b299-b51a007b63bb" class="bulleted-list"><li style="list-style-type:circle">컨텍스트 스위칭</li></ul></li></ul><ul id="300a50f5-227b-482f-adc6-a23291469d8e" class="bulleted-list"><li style="list-style-type:disc">병렬성<ul id="98ce4190-643b-4ae6-acc4-37519aaf8817" class="bulleted-list"><li style="list-style-type:circle">프로세서 하나에 코어 여러개 달려서 각각 동시에 작업 수행하는 것</li></ul><ul id="813c0aa8-41c5-4bd4-9b90-8b4b75154c3a" class="bulleted-list"><li style="list-style-type:circle">CPU나 스레드를 여러개 이용해서 병렬적으로 처리 하는 것</li></ul><ul id="37766c10-3dbb-44d2-a856-9a9354ff6576" class="bulleted-list"><li style="list-style-type:circle">듀얼코어 쿼드코어 옥타코어</li></ul></li></ul><h2 id="3b2a6f3c-6802-4cfd-aa20-abe545a79367" class="">Q2. 동기와 비동기에 대해 예시를 들어서 설명하세요.</h2><ul id="faa9283d-49e2-40e8-b31c-389286880bf9" class="bulleted-list"><li style="list-style-type:disc">동기 : 누군가에게 일을 부탁하고 끝날때까지 잠자코 기다리는 방식<ul id="07906142-ebdb-458a-b6c5-b5e635d4bc96" class="bulleted-list"><li style="list-style-type:circle">예) 게임 퀘스트<ul id="26edf556-0eb7-4f47-96a2-dcbb326ccbd5" class="bulleted-list"><li style="list-style-type:square">이전 퀘스트를 안깨면 다음 퀘스트를 못끝냄</li></ul></li></ul></li></ul><ul id="c9a95e15-b743-468f-9df4-5fccd64828ca" class="bulleted-list"><li style="list-style-type:disc">비동기 : 끝나면 말해 해놓고 다른 일을 하는것이 비동기<ul id="1ca8acee-d99f-4ae0-82f4-667d0b0dcb01" class="bulleted-list"><li style="list-style-type:circle">끝날 때까지 기다리지 않기 때문에 병렬로 다른 일을 할 수 있음</li></ul><ul id="fb2c69b6-11ba-4169-bd28-643a6c2a0a3d" class="bulleted-list"><li style="list-style-type:circle">예) 시험지를 여러장 나눠 주는 선생님<ul id="cb6c0d80-1ec8-4932-8609-43f0a7b91496" class="bulleted-list"><li style="list-style-type:square">선생님이 시험지를 나눠주는 동안 기다리는게 아니라 시험 문제를 계속 풀고 있을 수 있음</li></ul></li></ul><ul id="43ca425c-3740-40e6-ad87-a3991e09e288" class="bulleted-list"><li style="list-style-type:circle">의뢰한 일이 끝났는지 확인 하고 싶으면 별도의 방법 이용 - 콜백 url</li></ul></li></ul><p id="67d0f61e-9175-41fc-a48d-ddace9b98730" class="">
</p><h2 id="219c2646-80e2-4cd1-9b20-320bae980982" class="">Q3. 큐는 어디서 사용하는가? 예시 및 설명</h2><ul id="cd1007df-1740-48df-94e7-113db8e3c3ad" class="bulleted-list"><li style="list-style-type:disc">잡을 큐에 넣어두고 순차적으로 잡을 진행할 때 사용</li></ul><ul id="63ca9a9a-d0a3-4cba-97a2-35c2be81d865" class="bulleted-list"><li style="list-style-type:disc">여러처리가 동시에 진행되는 경우도 사용</li></ul><ul id="7c3c8908-6e4c-417a-b81d-9afebdc876cb" class="bulleted-list"><li style="list-style-type:disc">예시)<ul id="e64c3b2c-89f2-45c8-910b-fd7e9cbde1f5" class="bulleted-list"><li style="list-style-type:circle">메시지 큐<ul id="49bd010b-7a0d-4d93-91e4-23e71a1278a4" class="bulleted-list"><li style="list-style-type:square">프로세스 또는 프로그램 인스턴스가 데이터를 서로 교환할때 사용하는 방법</li></ul><ul id="c3adf333-5a0b-4043-b185-519c20e00691" class="bulleted-list"><li style="list-style-type:square"><strong>RabbitMQ</strong></li></ul></li></ul><ul id="27984f61-9768-4357-9b0e-a1f17be3e862" class="bulleted-list"><li style="list-style-type:circle">프로세스 스케쥴링 - 라운드 로빈 등</li></ul></li></ul><p id="2cd2abbf-c8d8-4ae8-bb7e-cdd66cd8f826" class="">
</p><h2 id="86fc0ce5-2f2b-40f4-b09b-84ce6c9819a9" class="">Q4. 데이터를 일관성 있게 유지 해야하는 이유와 사용 되는 알고리즘?</h2><ul id="a6eed49a-e4a1-4281-b203-b1f153bfc06d" class="bulleted-list"><li style="list-style-type:disc">배타적 제어<ul id="96c943fd-8b12-46c6-86f9-0bc5702bd034" class="bulleted-list"><li style="list-style-type:circle">복수의 처리가 공유 자원 (CPU, 메모리, 디스크)에 동시에 액세스 하면 불일치가 발생할수 있으므로 배타적 제어로 보호해야 함</li></ul></li></ul><ul id="1f864dff-31a2-46e9-820d-26e0f2245b36" class="bulleted-list"><li style="list-style-type:disc">예시) 세마포어, 뮤텍스<ul id="2702eb4d-ec48-41fc-bfe7-18fc1fb1576a" class="bulleted-list"><li style="list-style-type:circle">세마포어(Semaphore) : 공유된 자원의 데이터 혹은 임계영역(Critical Section) 등에 <strong>여러Process 혹은 Thread가 접근하는 것을 막아줌</strong>(즉, 동기화 대상이 하나 이상)</li></ul><ul id="7ed66e02-9020-46fc-bd88-7858cb7bc426" class="bulleted-list"><li style="list-style-type:circle">뮤텍스(Mutex) : 공유된 자원의 데이터 혹은 임계영역(Critical Section) 등에 <strong>하나의Process 혹은 Thread가 접근하는 것을 막아줌</strong>(즉, 동기화 대상이 하나)</li></ul><p id="f9328a92-2936-45ea-a121-91693a32e0f5" class="">
</p></li></ul><h2 id="9b41cc3f-a14f-413e-90f1-38e981990a46" class="">Q5. 인덱스는 몇번 탐색하는걸 권장 할까?</h2><ul id="a3796086-1274-435e-8b13-c685311aa71a" class="bulleted-list"><li style="list-style-type:disc">두번 탐색</li></ul><ul id="3c679b49-7558-474d-83db-a2da465cab2f" class="bulleted-list"><li style="list-style-type:disc">인덱스 리스트, 그 다음 컬렉션 순으로 탐색하기 때문. 관련 읽기 비용이 들게 됨.</li></ul><ul id="167db6e5-b76f-47dc-8b22-5e634bdc8276" class="bulleted-list"><li style="list-style-type:disc">컬렉션이 수정되었을 때 인덱스도 수정 되어야 함. </li></ul><ul id="a24375da-b9f7-48f7-89ff-59b8cbf0c14e" class="bulleted-list"><li style="list-style-type:disc">→ B트리의 높이를 균형있게 조절 하는 비용 + 데이터를 효율적으로 조회할 수 있게 분산시키는 비용도 들기 때문</li></ul></div></article></body></html>