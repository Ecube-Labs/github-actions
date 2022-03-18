## Example
<details>
<summary>.github/workflows/chromatic.yml</summary>

<pre>
name: 'Chromatic'

# NOTE: pull_request 트리거로 사용하면 안됨. https://www.chromatic.com/docs/turbosnap
on: ['push']

jobs:
  deployment:
    uses: Ecube-Labs/github-actions/.github/workflows/chromatic.yml@main
    secrets:
      projectToken: ${{ secrets.CHROMATIC_PROJECT_TOKEN }}
</pre>
</details>

<details>
<summary>.github/workflows/chromatic.yml (base branch: master)</summary>

<pre>
name: 'Chromatic'

# NOTE: pull_request 트리거로 사용하면 안됨. https://www.chromatic.com/docs/turbosnap
on: ['push']

jobs:
  deployment:
    uses: Ecube-Labs/github-actions/.github/workflows/chromatic.yml@master
    secrets:
      projectToken: ${{ secrets.CHROMATIC_PROJECT_TOKEN }}
</pre>
</details>
