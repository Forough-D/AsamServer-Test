<template>
  <div class="card h-100 mt-4">
    <div class="card-header pb-0 p-3">
      <div class="row">
        <div class="col-6 d-flex align-items-center">
          <h6 class="mb-0">My Invoices</h6>
        </div>
        <div class="col-6 text-end">
          <soft-button color="success" size="sm" variant="outline"
            >View All</soft-button
          >
        </div>
      </div>
    </div>
    <div class="card-body p-3 pb-0 mb-0">
      <ul class="list-group">
        <li
          class="list-group-item border-0 d-flex justify-content-between ps-0 mb-2 border-radius-lg"
        >
          <div class="d-flex flex-column">
            <h6 class="mb-1 text-dark font-weight-bold text-sm">
              March, 01, 2020
            </h6>
            <span class="text-xs">#26773</span>
          </div>
          <div class="d-flex align-items-center text-sm">
            $180
            <a href="/invoices/26772">
            <button class="btn btn-link text-dark text-sm mb-0 px-0 ms-4">
              <i class="fas fa-eye text-lg me-1" aria-hidden="true"></i>
              Show
            </button>
            </a>
          </div>
        </li>
        <li
          class="list-group-item border-0 d-flex justify-content-between ps-0 mb-2 border-radius-lg"
        >
          <div class="d-flex flex-column">
            <h6 class="text-dark mb-1 font-weight-bold text-sm">
              February, 10, 2021
            </h6>
            <span class="text-xs">#26772</span>
          </div>
          <div class="d-flex align-items-center text-sm">
            $250
            <a href="/invoices/26772">
              <button onclick="" class="btn btn-link text-dark text-sm mb-0 px-0 ms-4">
                <i class="fas fa-eye text-lg me-1" aria-hidden="true"></i>
                Show
              </button>
            </a> 
          </div>
        </li>
        <li
          class="list-group-item border-0 d-flex justify-content-between ps-0 mb-2 border-radius-lg"
        >
          <div class="d-flex flex-column">
            <h6 class="text-dark mb-1 font-weight-bold text-sm">
              April, 05, 2020
            </h6>
            <span class="text-xs">#26771</span>
          </div>
          <div class="d-flex align-items-center text-sm">
            $560
            <a href="/invoices/26772">
            <button class="btn btn-link text-dark text-sm mb-0 px-0 ms-4">
              <i class="fas fa-eye text-lg me-1" aria-hidden="true"></i>
              Show
            </button>
            </a>
          </div>
        </li>
        <li
          class="list-group-item border-0 d-flex justify-content-between ps-0 mb-2 border-radius-lg"
        >
          <div class="d-flex flex-column">
            <h6 class="text-dark mb-1 font-weight-bold text-sm">
              June, 25, 2019
            </h6>
            <span class="text-xs">#26770</span>
          </div>
          <div class="d-flex align-items-center text-sm">
            $120
            <a href="/invoices/26772">
            <button class="btn btn-link text-dark text-sm mb-0 px-0 ms-4">
              <i class="fas fa-eye text-lg me-1" aria-hidden="true"></i>
              Show
            </button>
            </a>
          </div>
        </li>
        <li
          class="list-group-item border-0 d-flex justify-content-between ps-0 border-radius-lg"
        >
          <div class="d-flex flex-column">
            <h6 class="text-dark mb-1 font-weight-bold text-sm">
              March, 01, 2019
            </h6>
            <span class="text-xs">#26769</span>
          </div>
          <div class="d-flex align-items-center text-sm">
            $300
            <a href="/invoices/26772">
            <button class="btn btn-link text-dark text-sm mb-0 px-0 ms-4">
              <i class="fas fa-eye text-lg me-1" aria-hidden="true"></i>
              Show
            </button>
            </a>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import SoftButton from "@/components/SoftButton.vue";

export default {
  name: "InvoiceCard",
  components: {
    SoftButton,
  },
};
</script>
