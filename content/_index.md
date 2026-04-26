---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      headings:
        about: '关于我'
        education: '教育背景'
        interests: '研究兴趣'
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 研究领域'
      subtitle: ''
      text: |-
        目前的研究工作聚焦于具身智能、数字人文与大语言模型的应用，包括家政机器人、非遗古琴数字化研究、基于大模型的多智能体协作、AI 生成内容检测等。希望能够利用具身智能技术解放人的双手，剥离人的工具意义，帮助人类专注于个性化价值的实现；追求利用数字化技术，为传统文化的数字化保护与传播提供新的工具。

        虽然目前发表成果仍然不算显赫，但在国家社科基金、国家自科基金以及地方政务系统建设等项目中的多年实践，让我积累了一定的一线经验。我期待在教学与科研中，与学生一起在真实问题和开放数据中持续打磨能力，在踏实的工作中一点点“长出来”有价值的成果。
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: 代表工作
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: 近期发表
      text: ''
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
---
