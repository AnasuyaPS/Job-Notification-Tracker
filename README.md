# Job-Notification-Tracker
import TopBar from "@/components/TopBar";
import ContextHeader from "@/components/ContextHeader";
import PrimaryWorkspace from "@/components/PrimaryWorkspace";
import SecondaryPanel from "@/components/SecondaryPanel";
import ProofFooter from "@/components/ProofFooter";

const Index = () => {
  return (
    <div className="flex min-h-screen flex-col bg-background">
      <TopBar
        projectName="KodNest Premium Build System"
        currentStep={1}
        totalSteps={5}
        status="in-progress"
      />

      <ContextHeader
        headline="Design System Reference"
        subtext="Every component, color, and spacing value in one place. Use this as the single source of truth for all screens built with the KodNest Premium Build System."
      />

      <main className="flex flex-1 flex-col gap-8 px-8 py-8 lg:flex-row">
        <div className="flex-[7] min-w-0">
          <PrimaryWorkspace />
        </div>
        <div className="flex-[3] lg:max-w-xs">
          <SecondaryPanel />
        </div>
      </main>

      <ProofFooter />
    </div>
  );
};

export default Index;
