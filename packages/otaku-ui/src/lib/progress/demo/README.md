---
import:
  import { Progress, Grid, GridItem } from 'otaku-ui'
---

[[toc]]

## Progress 进度条

::: demo

```tsx
<Progress></Progress>
```
:::

## 自定义文字

::: demo

```tsx
<Progress>10%</Progress>
```
:::


## 进度条内显示文字

::: demo

```tsx
<Progress inner percentage={50}>50%</Progress>
```
:::

## 自定义颜色

::: demo

```tsx
<Progress inner percentage={50} color="red">50%</Progress>
```
:::

## 垂直的进度条

::: demo

```tsx
<Grid>
  <GridItem>
    <Progress inner percentage={50} color="red" direction="vertical">50%</Progress>
  </GridItem>
  <GridItem>
    <Progress percentage={50}  direction="vertical">50%</Progress>
  </GridItem>
</Grid>

```
:::

## 圆形进度条

::: demo

```tsx
<Grid>
  <GridItem>
    <Progress percentage={50}  type="circle">50%</Progress>
  </GridItem>
  <GridItem>
    <Progress percentage={20}  type="circle">20%</Progress>
  </GridItem>
  <GridItem>
    <Progress percentage={90}  type="circle" >90%</Progress>
  </GridItem>
</Grid>

```
:::

## API

```ts
interface ProgressProps {
  inner?: boolean
  percentage?: number
  max?: number
  color?: string
  type?: 'circle'
  direction?: 'vertical' | 'horizontal'
  lineWidth?: number
  children?: string
}
```