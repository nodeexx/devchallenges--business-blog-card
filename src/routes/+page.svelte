<script lang="ts">
import * as Avatar from '$lib/browser/shadcn-svelte/components/ui/avatar';
import * as Card from '$lib/browser/shadcn-svelte/components/ui/card';
</script>

<Card.Root class="w-[418px] rounded-[12px] border-none p-0 shadow-none">
  <Card.Content class="p-0">
    <div class="image__container relative">
      <img
        src="/images/hero-image-business-card.png"
        alt="Business meeting"
        class="w-full select-none rounded-t-[12px] object-cover"
        draggable="false"
      />
    </div>

    <div class="flex flex-col gap-3 px-8">
      <Card.Title
        class="font-title text-[24px] font-medium leading-normal text-challenge-black"
        >Perfect solution for small business</Card.Title
      >
      <Card.Description
        class="text-[16px] font-normal leading-normal text-challenge-dark-gray"
      >
        Small businesses need to generate leads to grow. You can use tools like
        Ringy.
      </Card.Description>
    </div>
  </Card.Content>
  <Card.Footer class="px-8 pb-6 pt-12">
    <div class="flex items-center gap-[6px]">
      <div
        class="rounded-full border-[8px] border-solid border-challenge-light-gray"
      >
        <Avatar.Root class="h-[36px] w-[36px]">
          <Avatar.Image
            src="/images/avatar-image-business-card.png"
            alt="Avatar"
          />
          <Avatar.Fallback>AB</Avatar.Fallback>
        </Avatar.Root>
      </div>
      <div class="flex flex-col gap-1">
        <span class="text-[16px] font-bold leading-none text-challenge-black"
          >Amy Burgess</span
        >
        <span
          class="text-[12px] font-semibold leading-none text-challenge-dark-gray"
          >Customer Manger, Solution Oy</span
        >
      </div>
    </div>
  </Card.Footer>
</Card.Root>

<style lang="postcss">
.image__container::after {
  content: '';
  position: absolute;
  left: 0;
  right: 0;
  bottom: -1px;
  height: 70px;
  background: url('/images/white-overlay.svg') no-repeat bottom;
}
</style>
