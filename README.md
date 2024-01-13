<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/spring-projects/spring-batch/blob/main/spring-batch-docs/modules/ROOT/assets/images/spring-batch.png"><img align="right" src="/spring-projects/spring-batch/raw/main/spring-batch-docs/modules/ROOT/assets/images/spring-batch.png" width="200" height="200" style="max-width: 100%;"></a></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-spring-batch-" class="anchor" aria-hidden="true" tabindex="-1" href="#spring-batch-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">春季批次</font></font><a href="https://github.com/spring-projects/spring-batch/actions/workflows/continuous-integration.yml"><img src="https://github.com/spring-projects/spring-batch/actions/workflows/continuous-integration.yml/badge.svg" alt="构建状态" style="max-width: 100%;"></a></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Spring Batch 是一个轻量级、全面的批处理框架，旨在支持开发对企业系统日常运营至关重要的健壮批处理应用程序。</font></font><a href="https://github.com/spring-projects/spring-framework"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Spring Batch 建立在人们从Spring 框架</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中了解的生产力、基于 POJO 的开发方法和一般易用性功能的基础上</font><font style="vertical-align: inherit;">，同时使开发人员在必要时可以轻松访问和利用更高级的企业服务。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您正在为 Batch 应用程序寻找运行时编排工具，或者需要管理控制台来查看当前和历史执行情况，请查看</font></font><a href="https://cloud.spring.io/spring-cloud-dataflow/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Spring Cloud Data Flow</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">它是一个编排工具，用于部署和执行基于数据集成的微服务，包括 Spring Batch 应用程序。</font></font></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-getting-started" class="anchor" aria-hidden="true" tabindex="-1" href="#getting-started"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">入门</font></font></h1>
<h2 tabindex="-1" dir="auto"><a id="user-content-two-minutes-tutorial" class="anchor" aria-hidden="true" tabindex="-1" href="#two-minutes-tutorial"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">两分钟教程</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这个快速教程向您展示如何设置一个最小的项目来使用 Spring Batch 运行简单的批处理作业。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在您最喜欢的 IDE 中，创建一个新的基于 Maven 的 Java 17+ 项目并添加以下依赖项：</font></font></p>
<div class="highlight highlight-text-xml notranslate position-relative overflow-auto" dir="auto"><pre>&lt;<span class="pl-ent">dependencies</span>&gt;
    &lt;<span class="pl-ent">dependency</span>&gt;
        &lt;<span class="pl-ent">groupId</span>&gt;org.springframework.batch&lt;/<span class="pl-ent">groupId</span>&gt;
        &lt;<span class="pl-ent">artifactId</span>&gt;spring-batch-core&lt;/<span class="pl-ent">artifactId</span>&gt;
        &lt;<span class="pl-ent">version</span>&gt;${LATEST_VERSION}&lt;/<span class="pl-ent">version</span>&gt;
    &lt;/<span class="pl-ent">dependency</span>&gt;
    &lt;<span class="pl-ent">dependency</span>&gt;
        &lt;<span class="pl-ent">groupId</span>&gt;org.hsqldb&lt;/<span class="pl-ent">groupId</span>&gt;
        &lt;<span class="pl-ent">artifactId</span>&gt;hsqldb&lt;/<span class="pl-ent">artifactId</span>&gt;
        &lt;<span class="pl-ent">version</span>&gt;${LATEST_VERSION}&lt;/<span class="pl-ent">version</span>&gt;
        &lt;<span class="pl-ent">scope</span>&gt;runtime&lt;/<span class="pl-ent">scope</span>&gt;
    &lt;/<span class="pl-ent">dependency</span>&gt;
&lt;/<span class="pl-ent">dependencies</span>&gt;</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="<dependencies>
    <dependency>
        <groupId>org.springframework.batch</groupId>
        <artifactId>spring-batch-core</artifactId>
        <version>${LATEST_VERSION}</version>
    </dependency>
    <dependency>
        <groupId>org.hsqldb</groupId>
        <artifactId>hsqldb</artifactId>
        <version>${LATEST_VERSION}</version>
        <scope>runtime</scope>
    </dependency>
</dependencies>" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">然后，创建一个配置类来定义作业存储库将使用的数据源和事务管理器：</font></font></p>
<div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">import</span> <span class="pl-s1">javax</span>.<span class="pl-s1">sql</span>.<span class="pl-s1">DataSource</span>;

<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">context</span>.<span class="pl-s1">annotation</span>.<span class="pl-s1">Bean</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">context</span>.<span class="pl-s1">annotation</span>.<span class="pl-s1">Configuration</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">jdbc</span>.<span class="pl-s1">support</span>.<span class="pl-s1">JdbcTransactionManager</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">jdbc</span>.<span class="pl-s1">datasource</span>.<span class="pl-s1">embedded</span>.<span class="pl-s1">EmbeddedDatabaseBuilder</span>;

<span class="pl-c1">@</span><span class="pl-c1">Configuration</span>
<span class="pl-k">public</span> <span class="pl-k">class</span> <span class="pl-smi">DataSourceConfiguration</span> {

	<span class="pl-c1">@</span><span class="pl-c1">Bean</span>
	<span class="pl-k">public</span> <span class="pl-smi">DataSource</span> <span class="pl-en">dataSource</span>() {
		<span class="pl-k">return</span> <span class="pl-k">new</span> <span class="pl-smi">EmbeddedDatabaseBuilder</span>()
			.<span class="pl-en">addScript</span>(<span class="pl-s">"/org/springframework/batch/core/schema-hsqldb.sql"</span>)
			.<span class="pl-en">build</span>();
	}

	<span class="pl-c1">@</span><span class="pl-c1">Bean</span>
	<span class="pl-k">public</span> <span class="pl-smi">JdbcTransactionManager</span> <span class="pl-en">transactionManager</span>(<span class="pl-smi">DataSource</span> <span class="pl-s1">dataSource</span>) {
		<span class="pl-k">return</span> <span class="pl-k">new</span> <span class="pl-smi">JdbcTransactionManager</span>(<span class="pl-s1">dataSource</span>);
	}

}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="import javax.sql.DataSource;

import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.jdbc.support.JdbcTransactionManager;
import org.springframework.jdbc.datasource.embedded.EmbeddedDatabaseBuilder;

@Configuration
public class DataSourceConfiguration {

	@Bean
	public DataSource dataSource() {
		return new EmbeddedDatabaseBuilder()
			.addScript(&quot;/org/springframework/batch/core/schema-hsqldb.sql&quot;)
			.build();
	}

	@Bean
	public JdbcTransactionManager transactionManager(DataSource dataSource) {
		return new JdbcTransactionManager(dataSource);
	}

}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在本教程中，</font><font style="vertical-align: inherit;">使用 Spring Batch 的元数据表创建并初始化嵌入式</font></font><a href="http://www.hsqldb.org" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">HSQLDB数据库。</font></font></a><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">最后，创建一个类来定义批处理作业：</font></font></p>
<div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">Job</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">JobParameters</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">Step</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">configuration</span>.<span class="pl-s1">annotation</span>.<span class="pl-s1">EnableBatchProcessing</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">job</span>.<span class="pl-s1">builder</span>.<span class="pl-s1">JobBuilder</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">launch</span>.<span class="pl-s1">JobLauncher</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">repository</span>.<span class="pl-s1">JobRepository</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">core</span>.<span class="pl-s1">step</span>.<span class="pl-s1">builder</span>.<span class="pl-s1">StepBuilder</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">batch</span>.<span class="pl-s1">repeat</span>.<span class="pl-s1">RepeatStatus</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">context</span>.<span class="pl-s1">ApplicationContext</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">context</span>.<span class="pl-s1">annotation</span>.<span class="pl-s1">AnnotationConfigApplicationContext</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">context</span>.<span class="pl-s1">annotation</span>.<span class="pl-s1">Bean</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">context</span>.<span class="pl-s1">annotation</span>.<span class="pl-s1">Configuration</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">context</span>.<span class="pl-s1">annotation</span>.<span class="pl-s1">Import</span>;
<span class="pl-k">import</span> <span class="pl-s1">org</span>.<span class="pl-s1">springframework</span>.<span class="pl-s1">jdbc</span>.<span class="pl-s1">support</span>.<span class="pl-s1">JdbcTransactionManager</span>;

<span class="pl-c1">@</span><span class="pl-c1">Configuration</span>
<span class="pl-c1">@</span><span class="pl-c1">EnableBatchProcessing</span>
<span class="pl-c1">@</span><span class="pl-c1">Import</span>(<span class="pl-smi">DataSourceConfiguration</span>.<span class="pl-k">class</span>)
<span class="pl-k">public</span> <span class="pl-k">class</span> <span class="pl-smi">HelloWorldJobConfiguration</span> {

	<span class="pl-c1">@</span><span class="pl-c1">Bean</span>
	<span class="pl-k">public</span> <span class="pl-smi">Step</span> <span class="pl-en">step</span>(<span class="pl-smi">JobRepository</span> <span class="pl-s1">jobRepository</span>, <span class="pl-smi">JdbcTransactionManager</span> <span class="pl-s1">transactionManager</span>) {
		<span class="pl-k">return</span> <span class="pl-k">new</span> <span class="pl-smi">StepBuilder</span>(<span class="pl-s">"step"</span>, <span class="pl-s1">jobRepository</span>).<span class="pl-en">tasklet</span>((<span class="pl-s1">contribution</span>, <span class="pl-s1">chunkContext</span>) -&gt; {
			<span class="pl-smi">System</span>.<span class="pl-s1">out</span>.<span class="pl-en">println</span>(<span class="pl-s">"Hello world!"</span>);
			<span class="pl-k">return</span> <span class="pl-smi">RepeatStatus</span>.<span class="pl-c1">FINISHED</span>;
		}, <span class="pl-s1">transactionManager</span>).<span class="pl-en">build</span>();
	}

	<span class="pl-c1">@</span><span class="pl-c1">Bean</span>
	<span class="pl-k">public</span> <span class="pl-smi">Job</span> <span class="pl-en">job</span>(<span class="pl-smi">JobRepository</span> <span class="pl-s1">jobRepository</span>, <span class="pl-smi">Step</span> <span class="pl-s1">step</span>) {
		<span class="pl-k">return</span> <span class="pl-k">new</span> <span class="pl-smi">JobBuilder</span>(<span class="pl-s">"job"</span>, <span class="pl-s1">jobRepository</span>).<span class="pl-en">start</span>(<span class="pl-s1">step</span>).<span class="pl-en">build</span>();
	}

	<span class="pl-k">public</span> <span class="pl-k">static</span> <span class="pl-smi">void</span> <span class="pl-en">main</span>(<span class="pl-smi">String</span>[] <span class="pl-s1">args</span>) <span class="pl-k">throws</span> <span class="pl-smi">Exception</span> {
		<span class="pl-smi">ApplicationContext</span> <span class="pl-s1">context</span> = <span class="pl-k">new</span> <span class="pl-smi">AnnotationConfigApplicationContext</span>(<span class="pl-smi">HelloWorldJobConfiguration</span>.<span class="pl-k">class</span>);
		<span class="pl-smi">JobLauncher</span> <span class="pl-s1">jobLauncher</span> = <span class="pl-s1">context</span>.<span class="pl-en">getBean</span>(<span class="pl-smi">JobLauncher</span>.<span class="pl-k">class</span>);
		<span class="pl-smi">Job</span> <span class="pl-s1">job</span> = <span class="pl-s1">context</span>.<span class="pl-en">getBean</span>(<span class="pl-smi">Job</span>.<span class="pl-k">class</span>);
		<span class="pl-s1">jobLauncher</span>.<span class="pl-en">run</span>(<span class="pl-s1">job</span>, <span class="pl-k">new</span> <span class="pl-smi">JobParameters</span>());
	}

}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="import org.springframework.batch.core.Job;
import org.springframework.batch.core.JobParameters;
import org.springframework.batch.core.Step;
import org.springframework.batch.core.configuration.annotation.EnableBatchProcessing;
import org.springframework.batch.core.job.builder.JobBuilder;
import org.springframework.batch.core.launch.JobLauncher;
import org.springframework.batch.core.repository.JobRepository;
import org.springframework.batch.core.step.builder.StepBuilder;
import org.springframework.batch.repeat.RepeatStatus;
import org.springframework.context.ApplicationContext;
import org.springframework.context.annotation.AnnotationConfigApplicationContext;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.context.annotation.Import;
import org.springframework.jdbc.support.JdbcTransactionManager;

@Configuration
@EnableBatchProcessing
@Import(DataSourceConfiguration.class)
public class HelloWorldJobConfiguration {

	@Bean
	public Step step(JobRepository jobRepository, JdbcTransactionManager transactionManager) {
		return new StepBuilder(&quot;step&quot;, jobRepository).tasklet((contribution, chunkContext) -> {
			System.out.println(&quot;Hello world!&quot;);
			return RepeatStatus.FINISHED;
		}, transactionManager).build();
	}

	@Bean
	public Job job(JobRepository jobRepository, Step step) {
		return new JobBuilder(&quot;job&quot;, jobRepository).start(step).build();
	}

	public static void main(String[] args) throws Exception {
		ApplicationContext context = new AnnotationConfigApplicationContext(HelloWorldJobConfiguration.class);
		JobLauncher jobLauncher = context.getBean(JobLauncher.class);
		Job job = context.getBean(Job.class);
		jobLauncher.run(job, new JobParameters());
	}

}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">本教程中的作业由打印“Hello world!”的单个步骤组成。</font><font style="vertical-align: inherit;">到标准输出。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您现在可以运行</font></font><code>main</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该类的方法</font></font><code>HelloWorldJobConfiguration</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">来启动作业。</font><font style="vertical-align: inherit;">输出应类似于以下内容：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>INFO: Finished Spring Batch infrastructure beans configuration in 8 ms.
INFO: Starting embedded database: url='jdbc:hsqldb:mem:testdb', username='sa'
INFO: No database type set, using meta data indicating: HSQL
INFO: No Micrometer observation registry found, defaulting to ObservationRegistry.NOOP
INFO: No TaskExecutor has been set, defaulting to synchronous executor.
INFO: Job: [SimpleJob: [name=job]] launched with the following parameters: [{}]
INFO: Executing step: [step]
Hello world!
INFO: Step: [step] executed in 10ms
INFO: Job: [SimpleJob: [name=job]] completed with the following parameters: [{}] and the following status: [COMPLETED] in 25ms
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="INFO: Finished Spring Batch infrastructure beans configuration in 8 ms.
INFO: Starting embedded database: url='jdbc:hsqldb:mem:testdb', username='sa'
INFO: No database type set, using meta data indicating: HSQL
INFO: No Micrometer observation registry found, defaulting to ObservationRegistry.NOOP
INFO: No TaskExecutor has been set, defaulting to synchronous executor.
INFO: Job: [SimpleJob: [name=job]] launched with the following parameters: [{}]
INFO: Executing step: [step]
Hello world!
INFO: Step: [step] executed in 10ms
INFO: Job: [SimpleJob: [name=job]] completed with the following parameters: [{}] and the following status: [COMPLETED] in 25ms" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 tabindex="-1" dir="auto"><a id="user-content-getting-started-guide" class="anchor" aria-hidden="true" tabindex="-1" href="#getting-started-guide"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">入门指南</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">本指南是一个更实际的教程，展示了一个典型的 ETL 批处理作业，该作业从平面文件读取数据、转换数据并将其写入关系数据库。</font><font style="vertical-align: inherit;">它是一个基于Spring Boot的Spring Batch项目。</font><font style="vertical-align: inherit;">您可以在此处找到入门指南：</font></font><a href="https://spring.io/guides/gs/batch-processing/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">创建批处理服务</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-samples" class="anchor" aria-hidden="true" tabindex="-1" href="#samples"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">样品</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以在这里找到几个可供尝试的示例：</font></font><a href="https://github.com/spring-projects/spring-batch/tree/main/spring-batch-samples"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Spring Batch Samples</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-getting-help" class="anchor" aria-hidden="true" tabindex="-1" href="#getting-help"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">寻求帮助</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您有疑问或支持请求，请在</font></font><a href="https://github.com/spring-projects/spring-batch/discussions"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GitHub 讨论上打开新讨论或在</font></font></a><font style="vertical-align: inherit;"></font><a href="https://stackoverflow.com/questions/tagged/spring-batch" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">StackOverflow</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
上提出问题</font><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请不要</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在</font></font></strong><font style="vertical-align: inherit;"></font><a href="https://github.com/spring-projects/spring-batch/issues"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">问题跟踪器</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上针对问题或支持请求创建问题</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">我们希望保留问题跟踪器</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">专门</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">用于错误报告和功能请求。</font></font></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-reporting-issues" class="anchor" aria-hidden="true" tabindex="-1" href="#reporting-issues"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">报告问题</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Spring Batch 使用</font></font><a href="https://github.com/spring-projects/spring-batch/issues"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GitHub Issues</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">来记录错误和功能请求。</font><font style="vertical-align: inherit;">如果您想提出问题，请遵循以下建议：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在打开问题之前，请搜索问题跟踪器以查看是否有人已经报告了该问题。</font><font style="vertical-align: inherit;">如果该问题尚不存在，请创建一个新问题。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请按照问题</font></font><a href="https://github.com/spring-projects/spring-batch/blob/main/.github/ISSUE_TEMPLATE/bug_report.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">报告模板</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在问题报告中提供尽可能多的信息。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您需要粘贴代码或包含堆栈跟踪，请在文本前后使用 Markdown 转义符 (```)。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对于重要的错误，请创建一个测试用例或一个复制问题的项目并将其附加到问题中，如</font></font><a href="https://github.com/spring-projects/spring-batch/blob/main/ISSUE_REPORTING.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">问题报告指南</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中详述。</font></font></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-reporting-security-vulnerabilities" class="anchor" aria-hidden="true" tabindex="-1" href="#reporting-security-vulnerabilities"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">报告安全漏洞</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请参阅我们的</font></font><a href="https://github.com/spring-projects/spring-batch/security/policy"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安全政策</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-building-from-source" class="anchor" aria-hidden="true" tabindex="-1" href="#building-from-source"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从源头构建</font></font></h1>
<h2 tabindex="-1" dir="auto"><a id="user-content-using-the-command-line" class="anchor" aria-hidden="true" tabindex="-1" href="#using-the-command-line"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用命令行</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 Github 主页上的 URL 克隆 git 存储库：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ git clone git@github.com:spring-projects/spring-batch.git
$ cd spring-batch
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ git clone git@github.com:spring-projects/spring-batch.git
$ cd spring-batch" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Maven 是用于 Spring Batch 的构建工具。</font><font style="vertical-align: inherit;">您可以使用以下命令构建项目：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ ./mvnw package
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ ./mvnw package" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您想对所有集成测试执行完整构建，请运行：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ ./mvnw verify
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ ./mvnw verify" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，一些集成测试基于 Docker，因此请确保在运行完整构建之前已启动并运行 Docker。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要生成参考文档，请运行以下命令：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ cd spring-batch-docs
$ ../mvnw antora:antora
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ cd spring-batch-docs
$ ../mvnw antora:antora" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">参考文档可以在 中找到</font></font><code>spring-batch-docs/target/anotra/site</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-using-docker" class="anchor" aria-hidden="true" tabindex="-1" href="#using-docker"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 Docker</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您想在 Docker 容器中构建项目，可以按以下步骤操作：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$&gt; docker run -it --mount type=bind,source="$(pwd)",target=/spring-batch maven:3-openjdk-17 bash
#&gt; cd spring-batch
#&gt; ./mvnw package
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$> docker run -it --mount type=bind,source=&quot;$(pwd)&quot;,target=/spring-batch maven:3-openjdk-17 bash
#> cd spring-batch
#> ./mvnw package" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这将安装您之前在容器内的主机上克隆的源代码。</font><font style="vertical-align: inherit;">如果您想在容器内处理源代码的副本（对主机没有副作用），您可以按以下步骤操作：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$&gt; docker run -it maven:3-openjdk-17 bash
#&gt; git clone https://github.com/spring-projects/spring-batch.git
#&gt; cd spring-batch
#&gt; ./mvnw package
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$> docker run -it maven:3-openjdk-17 bash
#> git clone https://github.com/spring-projects/spring-batch.git
#> cd spring-batch
#> ./mvnw package" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h1 tabindex="-1" dir="auto"><a id="user-content-contributing-to-spring-batch" class="anchor" aria-hidden="true" tabindex="-1" href="#contributing-to-spring-batch"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为 Spring Batch 做出贡献</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们欢迎任何形式的贡献！</font><font style="vertical-align: inherit;">您可以通过以下一些方式为该项目做出贡献：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">通过回答问题和加入辩论，</font><font style="vertical-align: inherit;">参与</font></font><a href="https://twitter.com/springbatch" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Twitter</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://github.com/spring-projects/spring-batch/discussions"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GitHub 讨论</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://stackoverflow.com/questions/tagged/spring-batch" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">StackOverflow上的 Spring Batch 社区。</font></font></a><font style="vertical-align: inherit;"></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">针对错误和新功能创建</font></font><a href="https://github.com/spring-projects/spring-batch/issues"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">问题</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，或者对您感兴趣的问题进行评论和投票。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">帮助我们重现标有</font></font><a href="https://github.com/spring-projects/spring-batch/labels/status%3A%20need-help-to-reproduce"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">状态的问题：需要帮助重现，</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">遵循</font></font><a href="https://github.com/spring-projects/spring-batch/blob/main/ISSUE_REPORTING.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">问题报告指南</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Github 用于社交编码：如果您想编写代码，我们鼓励通过拉取请求做出贡献。</font><font style="vertical-align: inherit;">如果您想以这种方式贡献代码，请熟悉此处概述的流程：</font></font><a href="https://github.com/spring-projects/spring-batch/blob/main/CONTRIBUTING.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">贡献者指南</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">关注</font></font><a href="https://spring.io" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">spring.io</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上的 Spring Batch 相关文章。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在我们接受拉取请求之前，我们需要您签署</font></font><a href="https://support.springsource.com/spring_committer_signup" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">贡献者协议</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">签署贡献者协议并不授予任何人对主存储库的提交权，但这确实意味着我们可以接受您的贡献，如果我们这样做，您将获得作者信用。</font><font style="vertical-align: inherit;">活跃的贡献者可能会被要求加入核心团队，并被赋予合并拉取请求的能力。</font></font></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-code-of-conduct" class="anchor" aria-hidden="true" tabindex="-1" href="#code-of-conduct"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">行为守则</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请参阅我们的</font></font><a href="https://github.com/spring-projects/.github/blob/main/CODE_OF_CONDUCT.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">行为准则</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h1 tabindex="-1" dir="auto"><a id="user-content-license" class="anchor" aria-hidden="true" tabindex="-1" href="#license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">执照</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="https://www.apache.org/licenses/LICENSE-2.0.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Spring Batch 是在Apache 2.0 许可证</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下发布的开源软件</font><font style="vertical-align: inherit;">。</font></font></p>
</article></div>
