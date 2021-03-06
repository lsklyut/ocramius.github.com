---
layout: post
title: ProxyManager 1.0.0 release and expected 1.x lifetime
category: PHP
tags: ["php", "proxy"]
year: 2014
month: 12
day: 12
published: true
summary: ProxyManager 1.0.0 has been released together with the expected support schedule for 1.x
description: ProxyManager 1.0.0 is finally released, and an expected lifetime for the 1.x series is also attached with it!
tweet: 543363692067565568
---

<p style="align: center;">
    <img
        src="https://raw.githubusercontent.com/Ocramius/ProxyManager/1.0.0/proxy-manager.png"
        alt="ProxyManager"
        width="25%"
    />
</p>

<p>
    Today I finally released version 
    <a href="https://github.com/Ocramius/ProxyManager/releases/tag/1.0.0" target="_blank">1.0.0</a> of the 
    <a href="http://ocramius.github.io/ProxyManager" target="_blank">ProxyManager</a>
</p>

<h3>Noticeable improvements since 0.5.2:</h3>

<ul>
    <li>
        <a href="https://github.com/Ocramius/ProxyManager/pull/108" target="_blank">
            Windows path length limitations are now mitigated
        </a>
    </li>
    <li>
        <a href="https://github.com/Ocramius/ProxyManager/pull/172" target="_blank">
            Proxy classes are now re-generated when the library version changes
        </a>
    </li>
    <li>
        <a href="https://github.com/Ocramius/ProxyManager/pull/182" target="_blank">
            Documentation has been moved to github pages
        </a> (Markdown documentation will be kept in sync)
    </li>
    <li>
        <a href="https://github.com/Ocramius/ProxyManager/pull/194" target="_blank">
            It is not possible to trigger fatal errors via code-generation anymore
        </a>
    </li>
</ul>

<h3>Planned maintenance schedule</h3>

<p>
    ProxyManager 1.x will be a maintenance-release only:
</p>

<ul>
    <li>
        I plan to fix bugs until <time datetime="2015-12-11">December 11, 2015</time>
    </li>
    <li>
        I plan to fix security issues until <time datetime="2016-12-11">December 11, 2016</time>
    </li>
</ul>

<p>
    No features are going to be added to ProxyManager 1.x: the current <code>master</code> branch will instead
    become the development branch for version <code>2.0.0</code>.
</p>

<h3>ProxyManager 2.0.0 targets</h3>

<p>
    ProxyManager 2.0.0 has following main aims:
</p>

<ul>
    <li>
        <a href="https://github.com/Ocramius/ProxyManager/issues/167" target="_blank">
            Drop PHP 5.3, 5.4 and HHVM 3.3 limitations, aiming only at next-generation PHP runtimes
        </a>
    </li>
    <li>
        <a href="https://github.com/Ocramius/ProxyManager/issues/159" target="_blank">
            Lazy Loading ghost objects should be property-based, even for private properties
        </a>
    </li>
    <li>
        Move documentation to RST, eventually using <a href="https://github.com/CouscousPHP" target="_blank">couscous</a>
    </li>
    <li>
        <a href="https://github.com/Ocramius/ProxyManager/issues/115" target="_blank">
            Complete
            <abbr title="Liskov substitution principle">LSP</abbr>
            compliance by avoiding overriding constructors in proxies
        </a>
    </li>
    <li>
        Compatibility with 
        <a href="https://github.com/doctrine/common/blob/559a805125524b0bb6742638784c2979a5c5e607/lib/Doctrine/Common/Proxy/AbstractProxyFactory.php" target="_blank">
            <code>Doctrine\Common\Proxy\AbstractProxyFactory</code>
        </a> to improve doctrine proxy logic in next generation data mappers
    </li>
    <li>
        Prototypal inheritance in PHP, which 
        <a href="https://github.com/Ocramius/ProxyManager/pull/103" target="_blank">was left un-merged</a>
        for a long time, and will likely be moved to a different library
    </li>
</ul>

<h3>Thank you!</h3>

<p>
    It wouldn't be a good 1.0.0 release without thanking all the contributors that helped with the project, 
    by providing patches, bug reports and their useful insights to the project. Here are the most notable ones: 
</p>

<ul>
    <li><a href="https://github.com/blanchonvincent" target="_blank">blanchonvincent</a></li>
    <li><a href="https://github.com/malukenho" target="_blank">malukenho</a></li>
    <li><a href="https://github.com/staabm" target="_blank">staabm</a></li>
    <li><a href="https://github.com/gws" target="_blank">gws</a></li>
    <li><a href="https://github.com/leedavis81" target="_blank">leedavis81</a></li>
    <li><a href="https://github.com/lisachenko" target="_blank">lisachenko</a></li>
    <li><a href="https://github.com/Pittiplatsch" target="_blank">Pittiplatsch</a></li>
</ul>
