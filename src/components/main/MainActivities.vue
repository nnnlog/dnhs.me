<script lang="ts" setup></script>

<template>
  <div class="header" style="margin-top: 6rem">
    {{ $t("main.activities.header") }}
  </div>
  <i18n-t
    class="sub-header detail"
    keypath="main.activities.algorithm.header"
    tag="div"
  >
    <template #duration>
      <span class="detail-value">
        {{ $t("main.activities.algorithm.duration") }}
      </span>
    </template>
  </i18n-t>
  <ul>
    <i18n-t
      class="detail semi-bold"
      keypath="main.activities.algorithm.icpc.icpcwf"
      tag="li"
    >
      <template #th>
        <sup>{{ $t("_number_format.th") }}</sup>
      </template>
      <template #duration>
        <span class="detail-value">
          {{ $t("main.activities.algorithm.icpc.icpcwf_duration") }}
        </span>
      </template>
    </i18n-t>
    <li class="none">
      <ul>
        <i18n-t
          class="detail"
          keypath="main.activities.algorithm.icpc.icpc2022"
          tag="li"
        >
          <template #rank>
            <sup>{{ $t("main.activities.algorithm.icpc.icpc2022_rank") }}</sup>
          </template>
          <template #duration>
            <span class="detail-value">
              {{ $t("main.activities.algorithm.icpc.icpc2022_duration") }}
            </span>
          </template>
        </i18n-t>
      </ul>
    </li>
    <i18n-t
      class="detail semi-bold"
      keypath="main.activities.algorithm.koi_ta.header"
      tag="li"
    >
      <template #duration>
        <span class="detail-value">
          {{ $t("main.activities.algorithm.koi_ta.duration") }}
        </span>
      </template>
    </i18n-t>
    <li class="none">
      <ul>
        <i18n-t
          class="detail"
          keypath="main.activities.algorithm.koi_ta.koi2024first"
          tag="li"
        >
          <template #st>
            <sup>{{ $t("_number_format.st") }}</sup>
          </template>
          <template #duration>
            <span class="detail-value">
              {{ $t("main.activities.algorithm.koi_ta.koi2024first_duration") }}
            </span>
          </template>
        </i18n-t>
        <i18n-t
          class="detail"
          keypath="main.activities.algorithm.koi_ta.ioi_camp"
          tag="li"
        >
          <template #duration>
            <span class="detail-value">
              {{ $t("main.activities.algorithm.koi_ta.ioi_camp_duration") }}
            </span>
          </template>
        </i18n-t>
      </ul>
    </li>
    <i18n-t
      class="detail"
      keypath="main.activities.algorithm.koi_award.first_general"
      tag="li"
    >
      <template #st>
        <sup>{{ $t("_number_format.st") }}</sup>
      </template>
      <template #th>
        <sup>{{ $t("_number_format.th") }}</sup>
      </template>
      <template #duration>
        <span class="detail-value">
          {{ $t("main.activities.algorithm.koi_award.first_duration") }}
        </span>
      </template>
    </i18n-t>
    <li class="bold">
      <router-link class="link" to="/activity/algorithm">
        <span>{{ $t("main.activities.algorithm.view_all") }}</span
        ><mdicon height="1.5rem" name="arrow-right" width="1.5rem" />
      </router-link>
    </li>
  </ul>
  <i18n-t
    class="sub-header detail"
    keypath="main.activities.software.header"
    style="margin-top: 2rem"
    tag="div"
  >
    <template #duration>
      <span class="detail-value">
        {{ $t("main.activities.software.duration") }}
      </span>
    </template>
  </i18n-t>
  <ul>
    <i18n-t
      class="detail semi-bold"
      keypath="main.activities.software.soma.header"
      tag="li"
    >
      <template #th>
        <sup>{{ $t("_number_format.th") }}</sup>
      </template>
      <template #duration>
        <span class="detail-value">
          {{ $t("main.activities.software.soma.duration") }}
        </span>
      </template>
    </i18n-t>
    <li class="none">
      <ul>
        <i18n-t keypath="main.activities.software.soma.project" tag="li">
          <template #detail>
            <router-link class="link" to="/project/codemap">
              {{ $t("main.activities.software.soma.project_detail")
              }}<mdicon height="1.5rem" name="arrow-right" width="1.5rem" />
            </router-link>
          </template>
        </i18n-t>
      </ul>
    </li>
  </ul>
</template>
