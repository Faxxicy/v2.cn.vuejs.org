# Vue 2 的长期技术支持 (LTS)、终止支持 (EOL) 及其延长版服务

<p class="info"><b>希望继续使用 Vue 2？</b>
如果你希望在 Vue 2 的终止支持时间 (2023 年 12 月 31 日) 之后仍然使用它，并且需要一个能够满足安全和浏览器兼容性要求的维护版本，请务必查看：[HeroDevs 对 Vue 2 的无限期支持](https://www.herodevs.com/support/nes-vue?utm_source=vuejs-org&utm_medium=link&utm_campaign=lts-faq)。
</p>

## Vue 2 的技术支持会持续多久？

Vue 2.7 是当前、同时也是最后一个 Vue 2.x 的次级版本更新。Vue 2.7 会以其发布日期，即 2022 年 7 月 1 日开始计算，提供 18 个月的长期技术支持 (LTS：long-term support)。在此期间，Vue 2 将会提供必要的 bug 修复和安全修复，但不再提供新特性。

**Vue 2 的终止支持时间是 2023 年 12 月 31 日**。在此之后，Vue 2 在已有的分发渠道 (各类 CDN 和包管理器) 中仍然可用，但不再进行更新，包括对安全问题和浏览器兼容性问题的修复等。

## 应对终止支持的几个选项

### 升级到 Vue 3

Vue 3 是当前 Vue 的最高主版本。它提供了更好的性能和更好的 TypeScript 支持，并拥有诸如 Teleport、Suspense 和模板语法可多个根元素等 Vue 2 中没有的新特性。

Vue 3 也存在一些和 Vue 2 不兼容的变更，所以该迁移工作依据项目情况需要一定程度的工作量。完整的细节详见 [Vue 3 迁移指南](https://v3-migration.vuejs.org/zh/)。

尽管存在不兼容的变更，Vue 两个主版本之间主要的 API 依然是共享的。所以团队仍然可以把 Vue 2 的相关知识带到 Vue 3 使用。长期来看，我们也会尽可能避免类似 Vue 2 和 Vue 3 之间的这种不兼容变更。兼容性和生态的稳定性将会是我们未来发布的最高优先考量。而新特性的引入也不会导致大的迁移。

### 升级还是不升级

是否升级到 Vue 3 高度取决于具体的项目细节。以下是一些一般性的指导原则：

1. 理解升级的收益。

   由于 2.7 使得两个主版本之间的开发体验差距已经不再那么明显了——升级的主要收益将是更好的 TypeScript 支持、更好的性能，以及访问 Vue 3 生态系统和未来的新特性。

   试问你自己的团队几个问题：这个应用是否稳定且运行良好？是否需要在未来持续开发新特性？是否存在只能通过升级来解决的痛点或瓶颈？如果应用稳定且没有因为 Vue 2 而遇到重大的痛点，那么升级可能并不值得。

2. 理解升级的成本。

   该应用是否基于一些难以兼容 Vue 3 的第三方依赖？该应用是否严重依赖于 Vue 2 和 Vue 3 之间的行为差异？团队是否能够分配专门的时间来进行升级？你可以试着花一些时间进行这些方面的初步研究并得出一个预估结论，然后将其与 (1) 中的预期收益进行比较。我们无法提供精确的公式，但希望这可以帮助你做出决策。

### 继续使用 Vue 2

有些团队可能鉴于有限的投入、预算、风险承受能力、或有不兼容 Vue 3 的依赖，而在此时间段内无法升级到 Vue 3。我们对此完全理解，并将确保继续使用 Vue 2 是完全可行的选项，即便在其终止支持之后。

#### 技术角度

从技术角度看，Vue 2 是一项稳定且实战考验过的技术。如果它现在可以很好地支持你的工作，我们相信在可预见的未来仍然如此。

此外，我们也已经把大部分 Vue 3 重要的特性移植回了 [Vue 2.7](/v2/guide/migration-vue-2-7.html)，包括组合式 API 和 `<script setup>`。这使得 Vue 2 的项目可以提升其可扩展性、充分利用生态系统中最新的库、以及为潜在的 Vue 3 升级机会做更好的准备。

Vue 2.7 也是在终止支持之前保持维护的版本，所以如果你打算留在 Vue 2，应该至少升级至 2.7。

#### 安全与合规

有些团队的主要顾虑可能来自于安全、合规和浏览器兼容性方面。

- 软件在终止支持之后通常不会修复新的安全问题。Vue 2 在过去尚未有过真正的安全问题的记录，但是你可能会需要一个版本来应对合规或公司政策问题。

- 如果你在向客户提供带有服务级别协议 (SLA：Service Level Agreement) 的应用，你*需要*在技术栈中避免使用终止支持的软件。

- 浏览器有时会发布一些会破坏老旧库的变更。这样的情况极少发生，但理论上难以完全避免。

为了解决以上顾虑，我们和业内的专家们合作推出了 **Vue 2 的延长版 LTS 服务**。该服务会提供 Vue 2 安全和浏览器兼容性相关问题的修复版本，且带有 SLA 协议。如果你希望在 Vue 2 的终止支持时间，即 2023 年 12 月 31 日之后，仍然使用它，一定要移步至：[学习更多关于 HeroDevs 对 Vue 2 的无限期支持](https://www.herodevs.com/support/nes-vue?utm_source=vuejs-org&utm_medium=link&utm_campaign=lts-faq)。