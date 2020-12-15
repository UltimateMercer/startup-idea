<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    style="display: block; width: auto !important; height: 0 !important"
  >
    <filter
      id="uv-blue-green"
      x="-10%"
      y="-10%"
      width="120%"
      height="120%"
      filterUnits="objectBoundingBox"
      primitiveUnits="userSpaceOnUse"
      color-interpolation-filters="sRGB"
    >
      <feColorMatrix
        type="matrix"
        values=".33 .33 .33 0 0
            .33 .33 .33 0 0
            .33 .33 .33 0 0
            0 0 0 1 0"
        in="SourceGraphic"
        result="colormatrix"
      />
      <feComponentTransfer in="colormatrix" result="componentTransfer">
        <feFuncR type="table" tableValues="0.07 0.39 0 0" />
        <feFuncG type="table" tableValues="0.07 0 0.59 1" />
        <feFuncB type="table" tableValues="0.07 1 1 0.78" />
        <feFuncA type="table" tableValues="0 1" />
      </feComponentTransfer>
      <feBlend
        mode="normal"
        in="componentTransfer"
        in2="SourceGraphic"
        result="blend"
      />
    </filter>
    <filter
      id="uv-green"
      x="-10%"
      y="-10%"
      width="120%"
      height="120%"
      filterUnits="objectBoundingBox"
      primitiveUnits="userSpaceOnUse"
      color-interpolation-filters="sRGB"
    >
      <feColorMatrix
        type="matrix"
        values=".33 .33 .33 0 0
            .33 .33 .33 0 0
            .33 .33 .33 0 0
            0 0 0 1 0"
        in="SourceGraphic"
        result="colormatrix"
      />
      <feComponentTransfer in="colormatrix" result="componentTransfer">
        <feFuncR type="table" tableValues="0.07 0.39 0" />
        <feFuncG type="table" tableValues="0.07 0 1" />
        <feFuncB type="table" tableValues="0.07 1 0.78" />
        <feFuncA type="table" tableValues="0 1" />
      </feComponentTransfer>
      <feBlend
        mode="normal"
        in="componentTransfer"
        in2="SourceGraphic"
        result="blend"
      />
    </filter>
    <filter
      id="black-white"
      x="-10%"
      y="-10%"
      width="120%"
      height="120%"
      filterUnits="objectBoundingBox"
      primitiveUnits="userSpaceOnUse"
      color-interpolation-filters="sRGB"
    >
      <feColorMatrix
        type="matrix"
        values=".33 .33 .33 0 0
            .33 .33 .33 0 0
            .33 .33 .33 0 0
            0 0 0 1 0"
        in="SourceGraphic"
        result="colormatrix"
      />
      <feComponentTransfer in="colormatrix" result="componentTransfer">
        <feFuncR type="table" tableValues="0.07 0.92" />
        <feFuncG type="table" tableValues="0.07 0.92" />
        <feFuncB type="table" tableValues="0.07 0.92" />
        <feFuncA type="table" tableValues="0 1" />
      </feComponentTransfer>
      <feBlend
        mode="normal"
        in="componentTransfer"
        in2="SourceGraphic"
        result="blend"
      />
    </filter>
  </svg>
</template>
<script>
export default {}
</script>
<style lang="scss">
.uv-blue-green {
  filter: url('#uv-blue-green');
}
.uv-green {
  filter: url('#uv-green');
}

.black-white {
  filter: url('#black-white');
}
</style>
