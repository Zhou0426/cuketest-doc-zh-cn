# 零基础实现BDD自动化测试

# 前言

自动化测试越来越成为软件或网站发布必不可少的一个步骤，一方面，软件的应用场景越来越多，另一方面终端用户对应用质量期望越来越高。例如一个手机应用，可以跨不同的平台，如iOS，安卓，就是同一个安卓平台，也有多个版本，以及多种不同的显示屏尺寸。它们的组合加起来就有几十种可能性。网站应用也是类似，一个网站可能同时要适配多种浏览器(Chrome、IE、FireFox、手机上的iOS、安卓浏览器）,多种显示屏尺寸等。手动测试很难胜任这些测试任务。

自动化测试听起来是个很有挑战性的任务，只是某些专业技术人员擅长。很长一段时间来的确是这样。从事自动化测试开发的程序员不但要会懂得编程；还要花大量的时间学习商业或某些开源的测试工具，了解它们的用法和特性，并学习其特殊的编程语言，例如用LoadRunner要了解C语言、用QTP(UFT)要了解VBScript，用Selenium的开发者常去了解Ruby或者Python。这些语言在开发应用时不常用到或已不太流行，意味着学习这些语言主要还是应用在测试领域，投入的时间成本带来的回报有限。如果学习一种开发语言，既可以用来开发应用软件、又可以开发自动化测试那是最理想的。

本书介绍了一些方法和工具、试图降低自动化测试的门槛，让非专业测试人员也能方便快捷的完成自动化测试的任务。同时会介绍系统做自动化测试的方法。测试开发会用到自然语言和JavaScript，自然语言用于描述测试用例，JavaScript用来编写测试代码。两者之间通过一定的语法关联起来。

自然语言的测试用例等于是测试文档，描述了应用软件的行为，测试代码用来验证这些行为。这就是现阶段越来越流行的**行为驱动开发**(Behavior Driven Development，BDD)。行为驱动开发能够保持文档和测试脚本的一致性，便于维护、也便于业务人员和技术人员沟通，始终保持应用软件的技术实现反映业务的需求。Cucumber是行为驱动开发最流行的一个框架，它使用自然语言描述的行为来驱动测试代码，也支持多种语言，如Ruby、Python、JavaScript、Java等。JavaScript的流行已经无需累述，据统计，JavaScript是github上项目用到最多的语言，前端开发的必备，由于node.js的出现，它可以用来做全栈开发，覆盖应用的前端和后端。使用JavaScript写自动化测试意味着应用开发人员可以同时胜任应用软件的开发和它的自动化测试。

CukeTest是一款自动化测试的开发工具，结合了Cucumber框架和JavaScript语言，提供了编辑自动化测试的便捷功能，例如自动生成框架代码，代码与自然语言之间定位的跳转，可视化的维护用例场景、验证脚本、可视化报表等功能。它的出现降低了自动化测试的难度。更重要的一点，它可以免费下载使用([http://cuketest.com](http://cuketest.com))。所以本书主要以CukeTest工具界面为例子介绍自动化测试。但请读者也了解到，如果您只想单独使用Cucumber框架和JavaScript，一样也可以完成测试任务，只是开发效率有一些差异。

CukeTest能够针对各种类型的应用做自动化测试

